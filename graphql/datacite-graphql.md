# DataCite GraphQL API

The DataCite GraphQL API provides a flexible query interface for retrieving DOI metadata and the broader research knowledge graph. It exposes the full DataCite metadata model through a typed schema, enabling clients to request precisely the fields they need across a wide range of scholarly resource types — including datasets, journal articles, preprints, books, dissertations, software, workflows, instruments, and more. The API supports traversal of relationships between works, persons, organizations, funders, repositories, and DataCite member institutions, making it well suited for building citation graphs, discovery tools, and research analytics applications.

Authentication is not required for read-only queries against public DOI metadata. The API currently supports queries and a limited set of mutations (creating and deleting claims, updating user profiles). Mutations require an authenticated session. The schema is introspectable and follows the GraphQL Relay connection pattern (edges, nodes, pageInfo, totalCount) throughout for paginated result sets.

The endpoint is served at `https://api.datacite.org/graphql`. Queries can be submitted via HTTP POST with a JSON body containing a `query` field (and optionally `variables`). The API returns JSON:API-compatible schema.org representations alongside native GraphQL types, allowing downstream consumers to use either format. Usage statistics and citation counts are embedded directly on work types and can be retrieved in the same round trip as metadata.

**Endpoint:** https://api.datacite.org/graphql

**Documentation:** https://support.datacite.org/docs/datacite-graphql-api-guide

**References:**
- Documentation: https://support.datacite.org/docs/datacite-graphql-api-guide
- GettingStarted: https://support.datacite.org/docs/graphql-api
