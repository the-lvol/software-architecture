# Microkernel Pattern
[[Adaptation View]]

TODO: RAW: Pattern: Microkernel
Consider a system family where different versions of a system need to be supported. In each
version, components can be composed in different ways and other details, such as the offered
services, public APIs, or user interfaces, might be different. Nonetheless, the system family
should be realized using a common architecture to ease software maintenance and foster reuse. A MICROKERNEL realizes services that all systems, derived from the system family, need and
a plug-and-play infrastructure for the system-specific services. Internal servers (not visible to
clients) are used to realize version-specific services and they are only accessed through the MICROKERNEL. On the other hand, external servers offer APIs and user interfaces to clients by
using the MICROKERNEL. External servers are the only way for clients to access the MICROKERNEL architecture
