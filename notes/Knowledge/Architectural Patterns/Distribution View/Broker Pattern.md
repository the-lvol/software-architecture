# Broker Pattern
[[Distribution View]]

TODO: RAW: Pattern: Broker
Distributed software system developers face many challenges that do not arise in single-process
software. One is the communication across unreliable networks. Others are the integration of
heterogeneous components into coherent applications, as well as the efficient use of networking
resources. If developers of distributed systems must overcome all these challenges within their
application code, they may lose their primary focus: to develop applications that efficiently
tackle their domain-specific problems.
A BROKER separates the communication functionality of a distributed system from its application functionality. The BROKER hides and mediates all communication between the objects or
components of a system. A BROKER consists of a client-side REQUESTOR [VKZ04] to construct
and forward invocations, as well as a server-side INVOKER [VKZ04] that is responsible for invoking the operations of the target remote object. A MARSHALLER [VKZ04] on each side of
the communication path handles the transformation of requests and replies from programminglanguage native data types into a byte array that can be sent over the transmission medium.
