# Interpreter Pattern
[[Language Extension View]]

TODO: RAW: Pattern: Interpreter
A language syntax and grammar needs to be parsed and interpreted within an application. The
language needs to be interpreted at runtime (i.e. using a compiler is not feasible).
An INTERPRETER for the language is provided, which provides both parsing facilities and an
execution environment. The program that needs to be interpreted is provided in form of scripts
which are interpreted at runtime. These scripts are portable to each platform realization of the
INTERPRETER. For instance, the INTERPRETER can define a class per grammar rule of the
language. The parser of the interpreter parses language instructions according to these rules and
invokes the interpretation classes. Many more complex INTERPRETER architectures exist
