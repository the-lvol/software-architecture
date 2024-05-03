# Language Extension View
The Language Extension View focuses on integrating parts of a system that are written in non-native languages with those that are native to the software/hardware environment.

## Key Concerns:
- Integration of Non-native Languages: Strategies for incorporating non-native language components into the system.
- Translation to Native Environment: Mechanisms for converting non-native parts into a form that the native environment can execute.
- Support for Portability and Modifiability: Ensuring the system can easily adapt to different environments and evolve.

## Components and Communication:
- Native and Non-native Parts: Represent different language components within the system.
- Interpreter Component: Translates non-native language components into the native environment.
- Connectors consist of data carrying program instructions in the non-native language and the internal state of the non-native part.

## Optimizations and Alternatives:
- Interpreters with Byte-code Compilers: Some interpreters optimize by compiling byte-code on the fly, blending elements of a virtual machine.
- [[Virtual Machine Pattern]] vs. [[Interpreter Pattern]]: Virtual machines require compilation before runtime, while interpreters allow runtime script interpretation.
- Rule-Based Systems: An alternative for integrating rule-based or logical languages, operating on the principle of dynamic instruction redirection.

## Architectural Foundation:
- Indirection Layer: Serves as the base for interpreters, virtual machines, and rule-based systems, enabling dynamic runtime redirection of language instructions or byte code.
- Component and connector structures of these patterns are similar to an indirection layer, hence not depicted separately in diagrams.

## Static Alternatives for Language Extensions:
- Discussed in the context of aspect-oriented composition frameworks, these include manipulating the parse tree (Parse Tree Interpreter) or byte-code (Byte-Code Manipulator) for language extension.
- The relationship between these static alternatives and aspect-oriented composition patterns is illustrated, providing a foundation for extending languages within a system's architecture.

This view outlines methods for seamlessly integrating and translating non-native language components within a software system, emphasizing the importance of interpreters, virtual machines, and rule-based systems in supporting the portability and modifiability of these integrations.
