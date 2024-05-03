# Remote Procedure Calls Pattern
[[Distribution View]]

TODO: RAW: Pattern: Remote Procedure Calls
Consider the case where you want to realize an EXPLICIT INVOCATION in a distributed setting.
The use of low-level network protocols requires developers to invoke the send and receive operations of the respective network protocol implementations. This is undesirable because the
network access code cannot be reused, low-level details are not hidden, and thus solutions are
hard to maintain and understand.
REMOTE PROCEDURE CALLS extend the well-known procedure call abstraction to distributed
systems. They aim at letting a remote procedure invocation behave as if it were a local invocation. Programs are allowed to invoke procedures (or operations) in a different process and/or on
a remote machine.
