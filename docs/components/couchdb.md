# CouchDB

[CouchDB](https://couchdb.apache.org/) is a clusterable, syncable document-based database system.

In combination with [PouchDB](https://pouchdb.com/) in the frontend and added authentication through funnel it is a
robust offline-first solution.

Its de facto the only solution that works for our use case and is free and open source.

## Authentication

Authentication is offloaded at funnel. JWT configuration with CouchDB is everything but straight forward,
and having a explicit reverse proxy gives greater control and reduces surface for attacks.

e.g. limitation of the user to its own database already on request level

> This also means CouchDB should not be exposed over the network in any case, which
> would have fatal consequences due to basically an "admin party mode"

## Structure

Every use gets his own database. To do this funnel provides an init endpoint which checks if the user database already
exists, if this is not the case one is created.

- Every user database is completely flat, allowing easier sync
- Document ids consist of entity type and id in format `entityType:uuid`
- Document know their type stored in `$entityType`

## Further resources

- [CouchDB](https://couchdb.com/)
- [PouchDB](https://pouchdb.com/)
