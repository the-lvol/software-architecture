# Interceptor Pattern
[[Adaptation View]]

TODO: RAW: Pattern: Interceptor
A framework offers a number of reusable services to the applications that extend it. These
services need to be updated in the future as the application domain matures and they should still
be offered by the framework, so that the application developers do not need to re-implement
them. Furthermore, the framework developer cannot predict all such future services at the point
of time where the framework is created, while application developers may not be able to add
unanticipated extensions to the framework, in case e.g. that the framework is a black-box.
An INTERCEPTOR is a mechanism for transparently updating the services offered by the frame-
work in response to incoming events. An application can register with the framework any num-
ber of INTERCEPTORS that implement new services. The framework facilitates this registration
through dispatchers that assign events to INTERCEPTORS. The framework also provides the ap-
plications with the means to introspect on the framework’s behavior in order to properly handle
the events.