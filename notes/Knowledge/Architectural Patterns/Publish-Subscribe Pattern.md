# Publish-Subscribe Pattern
[[Component Interaction View]]

TODO: RAW: Pattern: Publish-Subscribe
A component should be accessed or informed of a specific runtime event. Events are of different
nature than direct interactions as in CLIENT-SERVER or PEER-TO-PEER. Sometimes a number
of components should be actively informed (an announcement or broadcast), in other cases only
one specific component is interested in the event. In contrast to EXPLICIT INVOCATIONS, event
producers and consumers need to be decoupled for a number of reasons: to support locality of
changes; to locate them in different processes or machines; to allow for an arbitrary time period
between the announcement of interest in an event, and the actual triggering of the event. Still,
there must be a way to inform the interested components?
PUBLISH-SUBSCRIBE allows event consumers (subscribers) to register for specific events, and
event producers to publish (raise) specific events that reach a specified number of consumers.
The PUBLISH-SUBSCRIBE mechanism is triggered by the event producers and automatically
executes a callback-operation to the event consumers. The mechanism thus takes care of decoupling producers and consumers by transmitting events between them
