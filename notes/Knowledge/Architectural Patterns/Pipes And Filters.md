# Pipes And Filters
[[Data Flow View]]

TODO: Raw: Consider as in BATCH SEQUENTIAL the case where a complex task can be sub-divided into a
number of smaller tasks, which can be defined as a series of independent computations. Additionally the application processes streams of data, i.e. it transforms input data streams into output
data streams. This functionality should not be realized by one monolithic component because
this component would be overly complex, and it would hinder modifiability and reusability.
Furthermore, different clients require different variations of the computations, for instance, the
results should be presented in different ways or different kinds of input data should be provided.
To reach this goal, it must be possible to flexibly compose individual sub-tasks according to the
client’s demands.
In a PIPES AND FILTERS architecture a complex task is divided into several sequential subtasks. Each of these sub-tasks is implemented by a separate, independent component, a filter,
which handles only this task. Filters have a number of inputs and a number of outputs and they
are connected flexibly using pipes but they are never aware of the identity of adjacent filters.
Each pipe realizes a stream of data between two components. Each filter consumes and delivers
data incrementally, which maximizes the throughput of each individual filter, since filters can
potentially work in parallel. Pipes act as data buffers between adjacent filters. The use of PIPES
AND FILTERS is advisable when little contextual information needs to be maintained between
the filter components and filters retain no state between invocations. PIPES AND FILTERS can be
flexibly composed. However, sharing data between these components is expensive or inflexible.
There are performance overheads for transferring data in pipes and data transformations, and
error handling is rather difficult
