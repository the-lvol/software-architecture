# Software Architecture

## Definition
    The software architecture of a system is the set of structures needed to reason about the system, which comprises software elements, relations among them, and properties of both

## Implications
The above definition has a set of implications

### Architecture Is a Set of [[Software Structure]]s
There are three categories of [[Architectural Structure]]s

### Architecture Is an Abstraction
Software architectures consist of [[Software Structure]]s, and [[Software Structure]]s consist of elements and relations

An architecture focuses on the public parts of the e.g. the classes, and omits the private parts (the actual implementation), to provide an abstraction of the system. This abstraction is needed to reason about such complex systems

### Every Software System Has a Software Architecture
Every system can be shown to comprise elements and relations among them to support some type of reasoning. In the most trivial case, a system is itself a single element—an uninteresting and probably non-useful architecture, but an architecture nevertheless

It can also happen that nobody knows the source, there is no documentation, and the source code has been lost. This leaves us with the executing binary code. This shows the architecture of the code, but not its representation (see [[Architecture Documentation]] and [[Architecture Reconstruction]])

### Architecture Includes Behavior
Behavior is the interaction between elements which is a part of our definition (see [[Component-And-Connector Structure (C&C)]])

Some behavior is too fine-grained and shouldn't be considered, but if the behavior of an element influences another element or the acceptability of the system as a whole, it must be considered

### Not All Architectures Are Good Architectures
Self-explanatory, see [[Architecture Design]] and [[Architecture Evaluation]]

## Not All Sofware Is Architecture
A structure is architectural if it supports reasoning about the system and the system’s properties. The reasoning should be about an attribute of the system that is important to some stakeholder

## What Makes A Good Architecture?
There is no one-size-fits-all answer to what makes a good architecture, as it depends on the specific goals and context of the system.

However, some general rules of thumb should be followed when designing most architectures, such as considering modifiability, maintainability, and scalability

Two clusters of recommendation

### Process Recommendation
1. Single Architect/Small Team: Prioritize conceptual integrity with a single architect or a small, coordinated team with a technical leader. Maintain strong ties to developers to avoid impractical designs
2. Prioritize Quality Attributes: Ensure the architecture is driven by prioritized, well-specified quality attributes, not just functionality
3. Document Using Views: Employ views tailored to essential stakeholder concerns and the project timeline. Start with minimal documentation if needed, with later elaboration
4. Evaluate Architecture: Consistently assess the architecture's ability to deliver key quality attributes. Early evaluation offers the most benefits
5. Incremental Implementation: Enable incremental growth (don't do it all at once). A "skeletal" communication system allows integration over time and early problem-detection

### Product/Structural Recommendations
1. Information Hiding & Separation of Concerns: Use well-defined modules that encapsulate likely changes within well-defined, change-resistant interfaces
2. Use Existing Solutions: Employ known architectural patterns to address established quality attributes whenever possible
3. Tool/Product Independence: Avoid specific dependencies on commercial tools, or design for easy changes if absolutely necessary
4. Separate Data Producers & Consumers: Improve modifiability by keeping data production and consumption distinct
5. Components ≠ Modules: Don't conflate them – there might be many component instances of a single module, or multi-component threads
6. Flexibility in Processor Assignment: Facilitate flexible process-processor allocation even at runtime
7. Consistency: A few standard interaction methods throughout the system enhance understanding, speed, reliability, and ease of modification
8. Resource Contention Management: Identify and clearly manage resource contention areas, providing guidelines for developers (e.g., performance budgets, network usage)
