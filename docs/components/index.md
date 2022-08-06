# High level overview

ThymeSave consists of:

- [funnel](./funnel.md) - Backend proxy functionality and configuration
- [silverware](./silverware.md) - Frontend application, npm packages, builtin plugins
- [CouchDB](./couchdb.md) - Persisting data and syncing with PouchDB in frontend
- [Auth0](./auth0.md) - Managed OAuth2 service for authentication and authorization

The communication hierarchy is like this:

``` mermaid
graph TD;
silverware-->funnel
silverware--->Auth0
funnel-->CouchDB[CouchDB Cluster]
funnel-->External_Websites[External websites]
funnel-->Auth0
```
