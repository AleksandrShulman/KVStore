# KVStore
A simple KV store that demonstrates transactionality in a system with multiple clients.

Use cases include basic `set`/`get`/`delete`/`reset` (no-context operations), along with operations that use context and can have race conditions, 
such as increment and decrement. There will be future use cases where a user may be able to provide a UDF (`f(key...) -> (key, value)`).

This is written in Java because the integrations are well-tested.
A future version could use Java, especially for the UDF cases.

Purposes:
- Demonstrate a simple Thrift API
- Demonstrate good client/server decoupling
- Use latest Bazel build tooling
- Demonstrate different kinds of testing (unit, functional, semi-integration, integration, etc.)
