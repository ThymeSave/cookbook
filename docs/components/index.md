# High level overview

ThymeSave consists of:

- [funnel](https://github.com/ThymeSave/funnel) - Backend proxy functionality and configuration
- [silverware](https://github.com/ThymeSave/silverware) - Frontend application, npm packages, builtin plugins
- [CouchDB](https://couchdb.apache.org/) - Persisting data and syncing with PouchDB in frontend
- [Auth0](https://auth0.com/) - Managed OAuth2 service for authentication and authorization

The communication hierarchy is like this:

``` mermaid
graph TD;
silverware-->funnel
silverware--->Auth0
funnel-->CouchDB[CouchDB Cluster]
funnel-->External_Websites[External websites]
funnel-->Auth0
```
