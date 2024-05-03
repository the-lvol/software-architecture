# Shared Repository
[[Data Centered View]]

TODO: RAW: Pattern: Shared Repository
Data needs to be shared between components. In sequential architectures like LAYERS or PIPES
AND FILTERS the only way to share data between the components (layers or filters) is to pass
the information along with the invocation, which might be inefficient for large data sets. Also it
might be inefficient, if the shared information varies from invocation to invocation because the
components’ interfaces must be prepared to transmit various kinds of data. Finally the long-term
persistence of the data requires a centralized data management.
In the SHARED REPOSITORY pattern one component of the system is used as a central data
store, accessed by all other independent components. This SHARED REPOSITORY offers suitable
means for accessing the data, for instance, a query API or language. The SHARED REPOSITORY
must be scalable to meet the clients’ requirements, and it must ensure data consistency. It must handle problems of resource contention, for example by locking accessed data. The SHARED
REPOSITORY might also introduce transaction mechanisms.

