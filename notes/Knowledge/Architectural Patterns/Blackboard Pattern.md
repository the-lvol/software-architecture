## Blackboard Pattern
[[Data Centered View]]

TODO: RAW: Pattern: Blackboard
Consider the case where a SHARED REPOSITORY is needed for the shared data of a computation,
but no deterministic solution strategies are known. Examples are image recognition or speech
recognition applications. However, it should be possible to realize a solution for these types of
applications.
In a BLACKBOARD architecture the complex task is divided into smaller sub-tasks for which
deterministic solutions are known. The BLACKBOARD is a SHARED REPOSITORY that uses
the results of its clients for heuristic computation and step-wise improvement of the solution.
Each client can access the BLACKBOARD to see if new inputs are presented for further processing and to deliver results after processing. A control component monitors the blackboard and
coordinates the clients according to the state of the blackboard.

