# Client-Server Pattern
The components are the clients and the servers, and the connectors are protocols and messages they share to carry out the system’s work

[[Component Interaction View]]

TODO: RAW: Pattern: Client-Server
Two components need to communicate, and they are independent of each other, even running in
different processes or being distributed in different machines. The two components are not equal
peers communicating with each other, but one of them is initiating the communication, asking
for a service that the other provides. Furthermore, multiple components might request the same
service provided by a single component. Thus, the component providing a service must be able
to cope with numerous requests at any time, i.e. the component must scale well). On the other
hand, the requesting components using one and the same service might deal differently with the
results. This asymmetry between the components should be reflected in the architecture for the
optimization of quality attributes such as performance, shared use of resources, and memory
consumption.
The CLIENT-SERVER pattern distinguishes two kinds of components: clients and servers. The
client requests information or services from a server. To do so it needs to know how to access the server, that is, it requires an ID or an address of the server and of course the server’s interface.
The server responds to the requests of the client, and processes each client request on its own. It
does not know about the ID or address of the client before the interaction takes place. Clients are
optimized for their application task, whereas servers are optimized for serving multiple clients.
