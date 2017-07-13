## Open Referral Human Services Data API Specification

This is a working project for the Open Referral Human Services Data API Specification.

You can view the public side of this project: https://openreferral.github.io/api-specification/

Here is a summary of what we are consider currently as part of the specification, as we take in feedback from the community of provides, vendors, and other human services stake holders.

We are currently moving the API definition from v1.0 to v1.1, with a focus on ensuring the API covers 100% of the surface area for the Human Services Data Specification (HSDS). 

## API Definitions

* Here is OpenAPI for version 1.0 of the HSDA - https://openreferral.github.io/api-specification/definition/v10/
* Here is OpenAPI for version 1.1 of the HSDA - https://openreferral.github.io/api-specification/definition/

## Road Map 

### [v1.1](https://github.com/openreferral/api-specification/issues?q=is%3Aissue+is%3Aopen+label%3Av1.1)

- [Validation](https://github.com/openreferral/api-specification/issues/43) - Produce JSON schema for HSDS and HSDS, and publish API definition, and working HSDS/a API for validating.
- Finalize - Take any feedback from Slack, Github, Google Group, and Spreadsheet and finalize the release of HSDA v1.1
- [Use Cases](https://github.com/openreferral/api-specification/issues/44) - We need use cases for any possible scenario in which HSDS/A will be put to work.

### [v1.2](https://github.com/openreferral/api-specification/issues?q=is%3Aissue+is%3Aopen+label%3Av1.2)

- [/everything](https://github.com/openreferral/api-specification/issues/45) - add an /everything to each core resource, allowing access to all sub resouces.
- [/search](https://github.com/openreferral/api-specification/issues/46) - give search a different response that spans all objects.
- [Use Cases](https://github.com/openreferral/api-specification/issues/44) - We need use cases for any possible scenario in which HSDS/A will be put to work.

### [v1.3](https://github.com/openreferral/api-specification/issues?q=is%3Aissue+is%3Aopen+label%3Av1.3)

- [Error Codes](https://github.com/openreferral/api-specification/issues/47) - Establish a set of object definitions for returning errors as part of responses.
- [Status Code](https://github.com/openreferral/api-specification/issues/48) - Establish a set of status codes across all paths, and associate as reponses.
- [Use Cases](https://github.com/openreferral/api-specification/issues/44) - We need use cases for any possible scenario in which HSDS/A will be put to work.

## API Design Conversation - Ongoing

* [Domain Guidance](https://github.com/openreferral/api-specification/issues/41) - Thoughts about whether or not we should be offering domain guidance in the future. Not worried about for v1.1, but maybe later.
* [Versioning](https://github.com/openreferral/api-specification/issues/8) - Guidance for versioning each API and communicating about what is supported.
* [Paths](https://github.com/openreferral/api-specification/issues/27) - The discussion around creating paths.
* [Verbs](https://github.com/openreferral/api-specification/issues/26) - here is the thread for further discussions around verbs.
* [Actions](https://github.com/openreferral/api-specification/issues/24) - Preparing for the future when we have more actions to be taken.
* [Parameters](https://github.com/openreferral/api-specification/issues/24) - The parameters discussion issue.
* [Headers](https://github.com/openreferral/api-specification/issues/5) - The header discussions.
* [Body](https://github.com/openreferral/api-specification/issues/25) - Discussion around usage of the request body.
* [Pagination](https://github.com/openreferral/api-specification/issues/10) - Evolving on current approach to using page= and per_page=.
* [Body Usage](https://github.com/openreferral/api-specification/issues/25) - How we are using the body of each request.
* [Data Scope / Filtering](https://github.com/openreferral/api-specification/issues/22) - Discussions around how to filter data, allowing API consumers to search across the contents of any implementation.
* [Schema Scope / Filtering](https://github.com/openreferral/api-specification/issues/21) - Considering the design of simple, standard, or full schema responses that can fe specificed using a prefer header.
* [Path Scope / Filtering](https://github.com/openreferral/api-specification/issues/38) - This won't be in the API design per se, but in the documentation (APIs.json), allowing for grouping and filtering of available paths similar to schema and data above
* [Project Scope / Filtering](https://github.com/openreferral/api-specification/issues/40) - Adding the fourth dimension to this scope / filtering discussion, I'm proposing we dicuss how projects are defined and isolated, which can allow them to move forward at different rates, and be reflected in documentation, code, and other resources--allowing for filtering by consumers.
* [Sorting](https://github.com/openreferral/api-specification/issues/12) - How we are going to handle sorting.
* [Operation ID](https://github.com/openreferral/api-specification/issues/4) - Decision around the operationID for each unique path.
* [Response Structure](https://github.com/openreferral/api-specification/issues/6) - More conversation about how to structure responses.
* [Status Codes](https://github.com/openreferral/api-specification/issues/3) - Discussion around the status codes to return.
* [Hypermedia](https://github.com/openreferral/api-specification/issues/7) - Conversations around future hypermedia usage.
* [Content Negotiation](https://github.com/openreferral/api-specification/issues/39) - Augmenting other conversations, begin introducing content negotiation concepts to the discussion.

## Other

* [Taxonomy](https://github.com/openreferral/api-specification/issues/19) - Earlier conversations around taxonomy. I am considering the wider picture when it comes to taxonomy, and what is available via the API.
* [Metadata](https://github.com/openreferral/api-specification/issues/28) - Putting off metadata paths until there is more discussion about how this will work with API deployment and management infrastructure.
* [Approval & Feedback](https://github.com/openreferral/api-specification/issues/34) - Discussion around how we are going to allow for the approval, notificiation, and feedback system around any change to a record in the system.
* [Universal Unique IDs](https://github.com/openreferral/api-specification/issues/35) - How will we allow for a universal uniqud ID system for all organizations, locations, and services, providing some provenance on the origin of the record.
* [Messaging](https://github.com/openreferral/api-specification/issues/37) - Suggesting that we isolate the messaging guidance for APIs, setting a standard for how you communicate within a single implementation as well across implementations.
* [Webhooks](https://github.com/openreferral/api-specification/issues/35) - How will we allow for a universal uniqud ID system for all organizations, locations, and services, providing some provenance on the origin of the record.

## API Portal

* [Demo Portal and API](http://developer.open.referral.adopta.agency/) - The demo portal setup for the project running PHP Slim on AWS linux instance for the API, and the developer portal running on Github Pages.

## Vendors

I am evaluating a handful of vendors and their schema and APIs as part of moving forward the specification. Here are the vendors I'm looking at currently:

* [iCarol](http://www.icarol.com)
* [Vision Link](http://visionlink.org/)
* [Health Leads](https://healthleadsusa.org/)
* [AIRS](https://github.com/openreferral/api-specification/issues/17) - Comoparing their schema and API work to the HSDS/A spec. 

## Privacy

* [Data Privacy Conversation](https://github.com/openreferral/api-specification/issues/20#issuecomment-303550584) - The open issue discussing privacy concerns.

## API Management

* Public - All the GET paths are publicly available, with no metering on them beyond just server logs.
* Github - All the POST, PUT, and DELETE require an x-appid and x-appkey, which are a Github username and valid Github token for user who is contributor on the Github repository for the API implementation.
* Logging - I want to start coming up with guidance for logging, either as part of API structure, or offloaded to API management solutions.

## Future Considerations

* [Scheduling and Calendaring](https://github.com/openreferral/api-specification/issues/23) - Suggestions around evolving the regular and holiday scheduling to think about calendaring.

## Archived

* [GraphQL](https://github.com/openreferral/api-specification/issues/9) - Discussion around using GraphQL to allow for more advanced usage and querying.
