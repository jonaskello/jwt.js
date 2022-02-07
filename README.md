# jwt.js

JWT tokens signed using nkeys for Ed25519 for the NATS JavaScript ecosystem.

### Very Important Disclaimer

This repository provides an API to build NATS JWTs using JavaScript. However, at
this time it is _not_ a supported API. Use at your own risk.

One important take away from this project is that the purpose of the library is
for building JWTs, not to validate them exhaustively. This means that tokens
generated by this library are expected to be validated by a process that uses
the [NATS JWT Go library](github.com/nats-io/jwt). As that library is the one used by:

- [nats-server](github.com/nats-io/nats-server),
- [nats-account-server](github.com/nats-io/nats-account-server)
- [nsc](github.com/nats-io/nsc).

Under that context, ultimate validity of the JWT is delegated to one of the
above. Use of this library implies an agreement with the above disclaimer.

### API

The API of this library requires knowledge of the NATS JWT entities.


### How use it

For now please look at the tests, and investigate the source.
