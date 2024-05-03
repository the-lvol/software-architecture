# Message Queuing
[[Distribution View]]

TODO: RAW: Pattern: Message Queuing
Consider a situation similar to that of REMOTE PROCEDURE CALLS, but it is necessary to decouple the sender from the receiver to realize queuing of invocations. Queuing is necessary,
for instance, when temporal outages of the receiver should be tolerated or when heterogeneous
systems should be integrated. For instance, when a legacy system using BATCH SEQUENTIAL should be integrated into a distributed system, only one invocation can be handled at a time
by that system. Somewhere additional messages must be queued until the system is ready to
process the next message.
Messages are not passed from client to server application directly, but through intermediate
message queues that store and forward the messages. This has a number of consequences:
senders and receivers of messages are decoupled, so they do not need to know each other’s
location (perhaps not even the identity). A sender just puts messages into a particular queue
and does not necessarily know who consumes the messages. For example, a message might be
consumed by more than one receiver. Receivers consume messages by monitoring queues.
