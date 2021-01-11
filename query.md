## Query Design
We are suggesting the adoption of [the GitHub API query design](https://docs.github.com/en/free-pro-team@latest/rest/reference/search) with some modifications. The approach strikes a nice balance between simple and complex querying which is especially important for ensuring HSDA is consumable by the widest possible audience.

## Query Parameters
On all top level resources there will be the following query parameters available.

- query
- fields
- resources
- page
- per_page
- sort_by
- order
- format

This keeps the querying of organizations, locations, services, and contacts easily queryable by any level of user simply by adjusting the query parameters. However, if you are an advanced user, you can pass in complete queries using the following patterns--I am not entirely sure how to document this, so I am going to articulate with examples:

### Basics
You can articulate multiple query parameters using any field available in the HSDA schema. The only difference is you use a colon instead of equals, with transportation=bus in this statement:

- query=transportation:bus

You can also use a like, with this showing any url that is "like" .gov.

- query=url like:.gov

You can also do greater than or less than like in this example with date:

- valid_from:>2019-01-01
- valid_from:>=2019-01-01
- valid_from:<2019-01-01
- valid_from:<=2019-01-01

You can also to between ranges on a field like with this example:

valid_from:2019-01-01..2019-12-31

I am still working to document and add some of the other approaches used by Github.

## Work to be Done

- NOT - They have the ability to do NOT in two ways by explicitly saying it, or adding a - before property -- still trying to decide on simplest approach.
- Operators - I don't fully understand or agree with Github's approach to operators, and probably will use a SQL like pattern of AND / OR with usage of parenthesis.
