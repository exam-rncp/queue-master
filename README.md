[![ci](https://github.com/exam-rncp/queue-master/actions/workflows/main.yml/badge.svg)](https://github.com/exam-rncp/queue-master/actions/workflows/main.yml)
[![Coverage Status](https://coveralls.io/repos/github/exam-rncp/queue-master/badge.svg?branch=main)](https://coveralls.io/github/exam-rncp/queue-master?branch=main)

# DEPRECATED: queue-master

A microservices-demo service that provides reading from the shipping
queue. It will spawn new docker containers that simulate the shipping
process.

This build is built, tested and released by travis.

# Test

`./test/test.sh < python testing file >`. For example: `./test/test.sh
unit.py`

# Build

`GROUP=weaveworksdemos COMMIT=test ./scripts/build.sh`

# Push

`GROUP=weaveworksdemos COMMIT=test ./scripts/push.sh`


## Redesign

This service will shortly be redesigned.

- Remove docker container shipping like functionality. Was only to make
  a better demonstration on Scope.
- Read object from queue and provide feedback on status
- See microservices-demo/orders and microservices-demo/shipping
