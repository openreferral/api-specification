## Open Referral Human Services Data API Specification

This is a working project for the Open Referral Human Services Data API Specification.

You can view the public side of this project: https://openreferral.github.io/api-specification/

Here is a summary of what we are consider currently as part of the specification, as we take in feedback from the community of provides, vendors, and other human services stake holders.

We are currently moving the API definition from v1.0 to v1.1, with a focus on ensuring the API covers 100% of the surface area for the Human Services Data Specification (HSDS). 

## API Definitions

* Here is OpenAPI for version 1.0 of the HSDA - https://openreferral.github.io/api-specification/definition/v10/
* Here is OpenAPI for version 1.1 of the HSDA - https://openreferral.github.io/api-specification/definition/

## API Design

* [Versioning](https://github.com/openreferral/api-specification/issues/8) - Guidance for versioning each API and communicating about what is supported.
* [Paths](https://github.com/openreferral/api-specification/issues/27) - The discussion around creating paths.
* [Verbs](https://github.com/openreferral/api-specification/issues/26) - here is the thread for further discussions around verbs.
* [Actions](https://github.com/openreferral/api-specification/issues/24) - Preparing for the future when we have more actions to be taken.
* [Parameters](https://github.com/openreferral/api-specification/issues/24) - The parameters discussion issue.
* [Headers](https://github.com/openreferral/api-specification/issues/5) - The header discussions.
* [Body](https://github.com/openreferral/api-specification/issues/25) - Discussion around usage of the request body.
* [Pagination](https://github.com/openreferral/api-specification/issues/10) - Evolving on current approach to using page= and per_page=.
* [Body Usage](https://github.com/openreferral/api-specification/issues/25) - How we are using the body of each request.
* [Data Filtering](https://github.com/openreferral/api-specification/issues/22) - Discussions around how to filter data, allowing API consumers to search across the contents of any implementation.
* [Schema Filtering](https://github.com/openreferral/api-specification/issues/21) - Considering the design of simple, standard, or full schema responses that can fe specificed using a prefer header.
* [Sorting](https://github.com/openreferral/api-specification/issues/12) - How we are going to handle sorting.
* [Operation ID](https://github.com/openreferral/api-specification/issues/4) - Decision around the operationID for each unique path.
* [Response Structure](https://github.com/openreferral/api-specdification/issues/6) - More conversation about how to structure responses.
* [Status Codes](https://github.com/openreferral/api-specification/issues/3) - Discussion around the status codes to return.
* [Hypermedia](https://github.com/openreferral/api-specification/issues/7) - Conversations around future hypermedia usage.
* [GraphQL](https://github.com/openreferral/api-specification/issues/9) - Discussion around using GraphQL to allow for more advanced usage and querying.

## API Management

* Public - All the GET paths are publicly available, with no metering on them beyond just server logs.
* Github - All the POST, PUT, and DELETE require an x-appid and x-appkey, which are a Github username and valid Github token for user who is contributor on the Github repository for the API implementation.

## API Portal

* [Demo Portal and API](http://developer.open.referral.adopta.agency/) - The demo portal setup for the project running PHP Slim on AWS linux instance for the API, and the developer portal running on Github Pages.

## Privacy

* [Data Privacy Conversation](https://github.com/openreferral/api-specification/issues/20#issuecomment-303550584) - The open issue discussing privacy concerns.

## Vendors

I am evaluating a handful of vendors and their schema and APIs as part of moving forward the specification. Here are the vendors I'm looking at currently:

* [iCarol](http://www.icarol.com)
* [Vision Link](http://visionlink.org/)
* [Health Leads](https://healthleadsusa.org/)
* [AIRS](https://github.com/openreferral/api-specification/issues/17) - Comoparing their schema and API work to the HSDS/A spec. 

## Other

* [Taxonomy](https://github.com/openreferral/api-specification/issues/19) - Earlier conversations around taxonomy. I am considering the wider picture when it comes to taxonomy, and what is available via the API.
* [Metadata](https://github.com/openreferral/api-specification/issues/28) - Putting off metadata paths until there is more discussion about how this will work with API deployment and management infrastructure.

## Future Considerations

* [Scheduling and Calendaring](https://github.com/openreferral/api-specification/issues/23) - Suggestions around evolving the regular and holiday scheduling to think about calendaring.
