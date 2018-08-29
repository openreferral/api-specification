## Open Referral Human Services Data API Specification

This project is driven by an OpenAPI definition located in [_data/api-commons/openapi-hsda.yaml](https://github.com/openreferral/api-specification/blob/master/_data/api-commons/openapi-hsda.yaml)

The website for this repo can be found at: https://openreferral.readthedocs.io/en/latest/hsda/

Here is the current road map for HSDA:

### [v1.3](https://github.com/openreferral/api-specification/issues?q=is%3Aissue+is%3Aopen+label%3Av1.3)

- [Error Codes](https://github.com/openreferral/api-specification/issues/47) - Establish a set of object definitions for returning errors as part of responses.
- [Status Code](https://github.com/openreferral/api-specification/issues/48) - Establish a set of status codes across all paths, and associate as reponses.

Use the Github issues for any questions and support.

The focus is primarily on the Human Services Data API (HSDA), but this work has been broken up into separate projects, to allow for separate of concerns, and versioning. You can find each project labeled:

- [hsda](https://github.com/openreferral/api-specification/labels/hsda) - The primary human services specification.
- [hsda search](https://github.com/openreferral/api-specification/labels/hsda-search) - Just for searching.
- [hsda bulk](https://github.com/openreferral/api-specification/labels/hsda-bulk) - Just for bulk management.
- [hsda meta](https://github.com/openreferral/api-specification/labels/hsda-meta) - Just for meta, system.
- [hsda taxonomy](https://github.com/openreferral/api-specification/labels/hsda-taxonomy) - Just for taxonomy.
- [hsda management](https://github.com/openreferral/api-specification/labels/hsda-management) - Just for management
- [hsda orchestration](https://github.com/openreferral/api-specification/labels/hsda-orchestration) - Just for orchestration (webhooks, events, jobs)
- [hsda utility](https://github.com/openreferral/api-specification/labels/hsda-utility) - All utility features.
- [hsda aggregation](https://github.com/openreferral/api-specification/labels/hsda-aggregation) - Upcoming aggregation work, acros multiple instances.
- [hsda custom](https://github.com/openreferral/api-specification/labels/hsda-custom) - Allowing for custom fields.

These are separate projects to allow for them to be moved forward separately. They are also meant to act as separate microservices, that can be deployed, scaled, and managed indepedent of each other while still working in concert.

Change Log:

### [v1.2](https://github.com/openreferral/api-specification/issues?q=is%3Aissue+is%3Aopen+label%3Av1.2)

- [/complete](https://github.com/openreferral/api-specification/issues/45) - add an /everything to each core resource, allowing access to all sub resouces.
- [query](query) - Shifting query parameter to be array, allowing for multiple fields to be queried.
- [content negotiation](https://github.com/openreferral/api-specification/issues/39) - Allow for JSON, XML, and responses.
- [sorting](https://github.com/openreferral/api-specification/issues/12) - Adding sorting.
- [pagination](https://github.com/openreferral/api-specification/issues/10) - Adding pagination.

### [v1.1](https://github.com/openreferral/api-specification/issues?q=is%3Aissue+is%3Aopen+label%3Av1.1)

- [Validation](https://github.com/openreferral/api-specification/issues/43) - Produce JSON schema for HSDS and HSDS, and publish API definition, and working HSDS/a API for validating.
- Finalize - Take any feedback from Slack, Github, Google Group, and Spreadsheet and finalize the release of HSDA v1.1
