# C2 Pattern
[[User Interaction View]]

TODO: RAW: Pattern: C2
An interactive system is comprised of multiple components such as GUI widgets, conceptual
models of those widgets at various levels, data structures, renderers, and of course application
logic. The system may need to support several requirements such as: different implementation language of components, different GUI frameworks reused, distribution in a heterogeneous
network, concurrent interaction of components without shared address spaces, run-time reconfiguration, multi-user interaction. Yet the system needs to be designed to achieve separation of
concerns and satisfy its performance constraints.
The system is decomposed into a top-to-bottom hierarchy of concurrent components that interact
asynchronously by sending messages through explicit connectors. Components submit request
messages upwards in the hierarchy, knowing the components above, but they send notification
messages downwards in the hierarchy, without knowing the components lying beneath. Components are only connected with connectors, but connectors may be connected to both components
and other connectors. The purposes of connectors is to broadcast, route, and filter messages.
