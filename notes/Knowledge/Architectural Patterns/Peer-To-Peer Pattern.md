# Peer-To-Peer Pattern
[[Component Interaction View]]

TODO: RAW: Pattern: Peer-to-Peer
Consider a situation similar to that of a CLIENT-SERVER, but in contrast to CLIENT-SERVER,
there is no distinction between the components: each component might both provide services
and consume services. When a component provides a service it must perform well according to the demands of the requesting components. Each component must know how to access other
components.
In the PEER-TO-PEER pattern each component has equal responsibilities, in particular it may act
both as a client and as a server. Each component offers its own services (or data) and is able
to access the services in other components. The PEER-TO-PEER network consists of a dynamic
number of components. A PEER-TO-PEER component knows how to access the network. Before
a component can join a network, it must get an initial reference to this network. This is solved
by a bootstrapping mechanism, such as providing public lists of dedicated peers or broadcast
messages (using IMPLICIT INVOCATION) in the network announcing peers.
