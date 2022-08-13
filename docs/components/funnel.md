# Funnel

Funnel is the small backend service, responsible for:

- CouchDB requests and authorization based on JWTs
- Fetching remote content, acting as a very restricted CORS Proxy
- Providing bootstrap configuration for the frontend

## Basic concepts / ideology

- Should be as small as possible and handle everything the user cares about in silverware
  - Allows users to work offline for most cases and in best case daily usage
  - keep attack surface minimal
- Plugin architecture allows extending the backend without altering the core
  - provides easy extension for self-hosting
  - allows e.g. GDPR self-service etc. to be implemented
  - ca be combined with frontend plugin to make ThymeSave even more useful

## Further resources

- [API docs](https://funnel.docs.thymesave.app/)
- [GitHub repository](https://github.com/thymesave/funnel)
