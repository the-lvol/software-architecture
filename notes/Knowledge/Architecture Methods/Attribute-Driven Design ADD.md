# Attribute-Driven Design ADD
- ADD is a method developed by SEI, focusing on basing software architecture design on quality attribute requirements.
- Utilizes a recursive decomposition process, employing architectural tactics and patterns to meet quality attribute scenarios.
- Results in architectures documenting high-level design choices, functionality containers, and interactions via views (e.g., module decomposition, concurrency, deployment).

## Steps in ADD Method
1. Initial Decomposition:
Start with the whole system, ensuring all inputs (constraints, functional and quality requirements) are ready.

2. Module Refinement Process:
a. Identify architectural drivers from quality scenarios and functional requirements.
b. Select an architectural pattern that meets these drivers, identifying child modules for tactic implementation.
c. Instantiate modules, allocate functionality from use cases, and document using multiple views.
d. Define child module interfaces, documenting module interactions and constraints.
e. Verify and refine use cases and quality scenarios as constraints for further module decomposition or implementation.

3. Iterative Decomposition:
Repeat the refinement process for each module requiring further decomposition.

## Integration with SEI Architectural Design Activities
- Quality Attribute Workshop (QAW): Helps elicit quality attribute requirements.
- Views and Beyond (VaB): Documents architecture through various stakeholder-focused views.
- Architecture Tradeoff Analysis Method (ATAM): Offers guidance on design analysis and risk feedback.
- ADD integrates with organizational processes, including Rational Unified Process and Agile methods, to enhance architecture design.

## Importance
ADD is crucial for achieving desired quality, and business goals, and providing a functional framework through targeted architectural design.
