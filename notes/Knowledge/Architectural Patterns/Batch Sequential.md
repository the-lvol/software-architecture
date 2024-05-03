# Batch Sequential
[[Data Flow View]]

TODO: RAW: Consider a complex task that can be sub-divided into a number of smaller tasks, which can be
defined as a series of independent computations. This should not be realized by one monolithic
component because this component would be overly complex, and it would hinder modifiability
and reusability.
In a BATCH SEQUENTIAL architecture the whole task is sub-divided into small processing steps,
which are realized as separate, independent components. Each step runs to completion and then
calls the next sequential step until the whole task is fulfilled. During each step a batch of data is
processed and sent as a whole to the next step.
