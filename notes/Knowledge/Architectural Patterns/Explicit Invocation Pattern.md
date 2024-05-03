# Explicit Invocation Pattern
[[Component Interaction View]]

TODO: RAW: Pattern: Explicit Invocation
Consider a component, the client, which needs to invoke a service defined in another component,
the supplier. Coupling the client with the supplier in various ways is not only harmless but
often desirable. For example the client must know the exact network location of the component
which offers the service in order to improve performance; or the client must always initiate
the invocation itself; or the client must block, waiting for the result of the invocation, before
proceeding with its business; or the topology of the interacting clients and suppliers is known
beforehand and must remain fixed. How can these two components interact?
An EXPLICIT INVOCATION allows a client to invoke services on a supplier, by coupling them in
various respects. The decisions that concern the coupling (e.g. network location of the supplier)
are known at design-time. The client provides these design decisions together with the service
name and parameters to the EXPLICIT INVOCATION mechanism, when initiating the invocation.
The EXPLICIT INVOCATION mechanism performs the invocations and delivers the result to the
client as soon as it is computed. The EXPLICIT INVOCATION mechanism may be part of the
client and the server or may exist as an independent component.

