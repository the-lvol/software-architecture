# Intensity/Locality Thesis
    (i) Architectural specifications are [[Intensional Abstraction]] and non-local; 
    (ii) Design specifications are [[Intensional Abstraction]]  but  local; and 
    (iii) Implementation specifications are both extensional and local.

| Specification Type | [[Intensional Abstraction]]/Extensional | Local/Non-local |
|--------------------|------------------------|-----------------|
| Architectural (see [[Architecture]])      | [[Intensional Abstraction]]            | Non-local       |
| [[Design]]                                | [[Intensional Abstraction]]            | Local           |
| [[Implementation]]                        | Extensional                            | Local           |

Also see [[Non-Local Abstraction]]

## i


## ii
Design specifications aim to be both intensional and local, per the Intension/Locality thesis. While often defined informally, formal specifications apply to recognized designs, including design patterns, to validate this thesis.

### Design Patterns as Intensional and Local
- Definition: Design patterns encapsulate recurring solutions in specific contexts, abstracted from application specifics. They are considered intensional due to their potential for an unbounded number of implementations.
- Perception: Seen as "microarchitectures," design patterns apply to limited modules, suggesting their locality.
- Factory Method Example: Illustrates intensionality (unbounded implementations) and locality (application within a confined context) through its structure and constraints.

### Formal Specification with LePUS:
- Components: Defines sets of product classes, factory classes, and factory methods, along with their interrelations (e.g., Clan and Produce predicates).
- Corollary 2: Validates the Factory Method pattern as both intensional (due to the flexibility in class and method instantiation) and local (pattern instance persists across design model extensions).

## iii [[Implementation]]
TODO: Some missing structure about the [[Implementation]] note

- Programs' Nature: While programming constructs like C++ templates and Eiffel generics might seem intensional due to their generic nature, they are ultimately extensional within the context of design models.
- Corollary 1: C++ Templates as Extensional:
  - Example Analysis: A C++ program with templates demonstrates that it is interpreted by a single design model, highlighting its extensional characteristic.
  - Design Model Components: The design model for a templated C++ program includes specific class and method atoms, and relations like Generic and Instantiate, which define a precise and singular interpretation.

## Architectural

### Patterns
- [[Layered Pattern]]
- [[Pipes And Filters]]

#### [[Layered Pattern]]
- Proven to be intensional (can be satisfied by an unbounded number of programs) and non-local (the specification can be violated by adding new elements inappropriately across layers).


#### [[Pipes And Filters]]
- Identified as intensional and non-local, as the addition of unconnected components violates the architectural style.

#### [[Law Of Demeter]]
- Initial Concept: Introduced as a design heuristic to simplify modifications and reduce complexity by limiting the objects a method can send messages
- Analysis: Found to be both intensional (applicable in infinitely many instances) and non-local (violations can occur anywhere within a program).
- Conclusion: Despite its origins as a design rule, the Law of Demeter functions effectively as an architectural rule, necessitating widespread adherence and enforcement through architectural practices.


## UML
    An intensional specification ϕ is quasi-extensional if and only if the set of design models that satisfy ϕ, has a single lower bound with respect to the partial-ordering relation “subsumption”

    UML class diagrams are quasi-extensional
