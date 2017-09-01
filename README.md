## Open Referral Human Services Data API Specification

This project is driven by an OpenAPI definition located in [_data/api-commons/openapi.yaml](https://github.com/openreferral/api-specification/blob/master/_data/api-commons/openapi.yaml)

The website for this repo can be found at: https://openreferral.github.io/api-specification/definition/

Here is the current road map:

### [v1.1](https://github.com/openreferral/api-specification/issues?q=is%3Aissue+is%3Aopen+label%3Av1.1)

- [Validation](https://github.com/openreferral/api-specification/issues/43) - Produce JSON schema for HSDS and HSDS, and publish API definition, and working HSDS/a API for validating.
- Finalize - Take any feedback from Slack, Github, Google Group, and Spreadsheet and finalize the release of HSDA v1.1

### [v1.2](https://github.com/openreferral/api-specification/issues?q=is%3Aissue+is%3Aopen+label%3Av1.2)

- [/complete](https://github.com/openreferral/api-specification/issues/45) - add an /everything to each core resource, allowing access to all sub resouces.
- [query](query) - Shifting query parameter to be array, allowing for multiple fields to be queried.
- [content negotiation](https://github.com/openreferral/api-specification/issues/39) - Allow for JSON, XML, and responses.
- [sorting](https://github.com/openreferral/api-specification/issues/12) - Adding sorting.
- [pagination](https://github.com/openreferral/api-specification/issues/10) - Adding pagination.

### [v1.3](https://github.com/openreferral/api-specification/issues?q=is%3Aissue+is%3Aopen+label%3Av1.3)

- [Error Codes](https://github.com/openreferral/api-specification/issues/47) - Establish a set of object definitions for returning errors as part of responses.
- [Status Code](https://github.com/openreferral/api-specification/issues/48) - Establish a set of status codes across all paths, and associate as reponses.

All other conversations can be found under the Github issues for this repository. Feel free to submit an issue if you have any questions.

This project runs using Jekyll hosted on Github, with _data as the data source for the entire project, and other continuous integration workflows.
