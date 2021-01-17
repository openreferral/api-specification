## Open Referral Human Services Data API (HSDA)
This is the repository for managing the Open Referral Human Services Data API (HSDA), providing a common interface for accessing organizations, locations, services, and contacts for 211 human services information.

### Key Links

- [Open Referral Website](https://openreferral.org/)
- [HSDS Documentation](http://docs.openreferral.org/en/latest/hsds/)
- [HSDA Documentation](http://docs.openreferral.org/en/latest/hsda/)

### HSDA v2.0 OpenAPIs
HSDA uses the [OpenAPI specification](http://spec.openapis.org/oas/v3.0.3) to describe the surface area of the API, providing a machine readable definition for all of HSDA.

- **HSDA** ([OpenAPI on GitHub](https://github.com/openreferral/api-specification/blob/master/v2.0/openapi-hsda.yaml)) ([OpenAPI in Workspace](https://www.postman.com/api-evangelist/workspace/human-services-data-api-hsda/api/1a7abc09-be01-45fa-932c-7ed3d11e43ea?version=2c338c6f-4da0-452c-bb5d-ef834c1ce7cc&tab=overview)) ([Collection in Workspace](https://www.postman.com/api-evangelist/workspace/human-services-data-api-hsda/documentation/35240-b0c2834a-60ac-4076-87a9-aac143874f20))
- **HSDA Search** ([OpenAPI on GitHub](https://github.com/openreferral/api-specification/blob/master/v2.0/openapi-hsda-search.yaml)) ([OpenAPI in Workspace](https://www.postman.com/api-evangelist/workspace/human-services-data-api-hsda/api/eae721cd-11f6-4c46-824d-2775f5328561?version=5ad8f4f2-29af-4379-9c50-f8ecf2ba6e4b&tab=overview)) ([Collection Docs in Workspace](https://www.postman.com/api-evangelist/workspace/human-services-data-api-hsda/documentation/35240-e8cdaa8c-5444-4722-a6fd-181f120d49f3))
- **HSDA Meta** ([OpenAPI on GitHub](https://github.com/openreferral/api-specification/blob/master/v2.0/openapi-hsda-meta.yaml)) ([OpenAPI in Workspace](https://www.postman.com/api-evangelist/workspace/human-services-data-api-hsda/api/55b2862e-39c1-48e8-987f-e6c38df0323d?version=632b6e4c-f36c-473a-ad24-4b4e34cf410a&tab=overview)) ([Collection Docs in Workspace](https://www.postman.com/api-evangelist/workspace/human-services-data-api-hsda/documentation/35240-60e93ec1-23e9-4691-8a86-2d833dc2b896))
- **HSDA Taxonomy** ([OpenAPI on GitHub](https://github.com/openreferral/api-specification/blob/master/v2.0/openapi-hsda-taxonomy.yaml)) ([OpenAPI in Workspace](https://www.postman.com/api-evangelist/workspace/human-services-data-api-hsda/api/6fb08211-ff92-4923-a2fe-e000d9a86df9?version=2a3ed87a-1e53-460d-aec1-a5583910d2f1&tab=overview)) ([Collection Docs in Workspace](https://www.postman.com/api-evangelist/workspace/human-services-data-api-hsda/documentation/35240-fe401428-96ce-43c8-99a2-ca13929e71a5))

Drafts for v2.0 are currently being finalized and open for comments--here is how you can provide feedback:

- [GitHub Issues](https://github.com/openreferral/api-specification/issues) - You can submit a Github issue with your feedback or OpenAPI reference.
- [Postman API Comments](https://www.postman.com/api-evangelist/workspace/human-services-data-api-hsda/overview) - You can comment on each of the OpenAPI as well as each individual part of the API.

Using OpenAPI helps ground the conversation around each of the APIs being evolved here. It significantly helps to submit the OpenAPI snippet with suggested changes, or highlight and common on the portion of the OpenAPI you wish to provide feedback on. Feel free to all submit pull requests on OpenAPIs via Github, or collections via Postman.

You can follow along with work in [the public workspace for the HSDA APIs](https://www.postman.com/api-evangelist/workspace/human-services-data-api-hsda/overview) as we work to finalize and standardize the OpenAPIs for HSDA. Your feedback is appreciated.

### HSDA v2.0 Major Changes
Here are the highlights of the HSDA v2.0 update, with the focus being on HSDS upgrade, but using the opportunity to clean up some other areas of the HSDA specification.

- **HSDS v2.0 Update** - All of the schema were brought up to date with [version 2.0 of HSDS](https://docs.openreferral.org/en/latest/hsds/reference/).
- **Standardized Querying** - We standardized the search across contacts, locations, organizations, and services, as well as for search--[the query standard is outline here](https://github.com/openreferral/api-specification/blob/master/query.md).
- **Header Pagination** - A set of headers were added to each of the root level resources, showing you the details of pagination for each query.
- **Status Codes** - Status codes were standardized across all responses, providing a consistent set of HTTP status codes for all API paths.
- **RFC 7807 for Errors** - We standardized the error responses for 4xx and 5xx errors, providing a common approach to reporting problems using [RFC 7807 - Problem Details for HTTP APIs](https://tools.ietf.org/html/rfc7807).

The new standardized query structure dealt with a number of the issues that were submitted, while allowing for basic keyword search, as well as a much more complex approach that allows querying by any field, while also having full control over what gets returned.
