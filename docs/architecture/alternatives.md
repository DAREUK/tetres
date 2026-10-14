---
icon: lucide/table
title: Alternatives
---

# Alternatives

## X-Road[^1]

[^1]: Last reviewed 2026-10-13

> open-source software that enables unified, secure data exchange between organisations within a collaborative ecosystem. It streamlines data exchange processes, enhances security, and facilitates interoperability, enabling organisations to derive greater value from their data assets.

/// caption
https://x-road.global/
///

[X-Road](https://x-road.global/) requires a [Security Server](https://x-road.global/security) at each node.
It is a public internet-facing gateway through which all X-Road traffic enters or leaves the node.
It sends and receives encrypted (TLS) messages to and from security servers at other nodes.
The security server signs all messages that are sent, and the receiving security server validates messages.

The configuration for all security servers is managed by a [Central Server](https://x-road.global/architecture), which maintains a list of all security servers and ceritication authorities.

A major limitation of X-Road is all messages are synchronous.
REST and SOAP are the only [supported protocols](https://docs.x-road.global/Protocols/pr-messtransp_x-road_message_transport_protocol.html).

This is suitable for some forms of federation such as remote text-based queries, but will not support more complex TRE use cases.
For example, [GRPC is used by Flower AI](https://flower.ai/glossary/grpc) for federated learning; [websockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API) are often used for streaming which requires a persistent connection.
