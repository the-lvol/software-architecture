# Design Model
TODO: this note vs the [[Design]] note

- Purpose: Bridge architectural/design specifications with implementations by abstracting programs to a convenient representation.
- Example by Eden and Hirshfeld: Source code can be modeled as design models - first-order, finite structures in mathematical logic.
- Structure of Design Models: Consists of atoms (classes, methods) and relations among them, demonstrating the program's structural aspects relevant to software design theory.

## Case Study
- Java Program Abstraction: An example demonstrates the abstraction of an object-oriented program into classes and methods and their relations. E.g., `Inherit(BorderDecorator, Decorator)` shows the relation in inheritance.
- Limitations: Such models primarily focus on structural properties like class and method interdependencies, not dynamic properties (fairness, complexity).

## Specification
Definitions:
- SPEC: Represents the set of formal languages used for specifications.
- SPEC:* The set of all expressions made in any language within SPEC. A specification is an element of SPEC*.

Languages: Includes specification languages (e.g., Z, LePUS) and programming languages (e.g., Eiffel, ANSI C, C++, Java™).

### Evaluating Specifications:
- Main Question: Can we determine if a program satisfies a given specification?
- Use of Design Models: Design models serve as the semantics to evaluate if a program meets its specifications.

### Instances of Specifications:
- Example Specification: Inherit(x,y) - A specification that can be satisfied by any pair of atoms in the Inherit relation.
- Instance Example: The pair `〈BorderDecorator, Decorator〉` satisfies the specification, demonstrating an instance of the specification.
- Distinction: An instance is not the same as a program. A program may have zero, multiple, or any number of instances of a specification.

## Programs
    A program π satisfies a specification ϕ if the design model of π satisfies ϕ.

- Program Definition: A program is a specification associated with a single design model.
- Denotation Function (W): A function that maps each program (element ϕ in PW, a subset of SPEC*) to exactly one design model that satisfies ϕ.

### Properties and Examples:
- The domain of W: Contains programming language expressions, e.g., C++ and Eiffel.
- Illustrations: Figures and tables in the text show how programs in Java™ and C++ are denoted by specific design models.

### Key Observations:
- PW vs. SPEC:* PW (the set of all programs) is a small subset of SPEC* (all possible expressions in specification languages).
- Multiplicity: Many expressions in SPEC* can be satisfied by more than one design model, unlike programs that are associated with a single design model.
