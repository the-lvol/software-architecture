# Virtual Machine Pattern
[[Language Extension View]]

TODO: RAW: Pattern: Virtual Machine
An efficient execution environment for a programming language is needed. The architecture
should facilitate portability, code optimizations, and native machine code generation. Runtime
interpretation of the language is not necessarily required.
A VIRTUAL MACHINE defines a simple machine architecture on which not machine code but
an intermediate form called the byte-code can be executed. The language is compiled into that
byte-code. The VIRTUAL MACHINE can be realized on different platforms, so that the byte-code
can be portable between these platforms. The VIRTUAL MACHINE redirects invocations from a
byte-code layer into an implementation layer for the commands of the byte-code.

