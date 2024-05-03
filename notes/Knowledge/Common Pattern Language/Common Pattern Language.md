# Common Pattern Language
Aim: To establish common ground in the architectural patterns community.

Approach: Propose a pattern language that integrates existing architectural patterns and styles, focusing on the relationships between them to offer a comprehensive overview.

## Key Strategies
- Unification of Concepts: Treats architectural patterns and styles as fundamentally similar, merging them into a single pattern language. This includes classical patterns (e.g., from POSA) and styles (e.g., from SEI), emphasizing their interconnections.
- Simplification: Uses the term "architectural pattern" throughout to avoid complexity, acknowledging some patterns may seem obvious but are included for their contribution to the overall understanding.
- Architectural Level Focus: Defines a pattern as architectural if it addresses the system's overall structure rather than specific subsystems, with an exception for the INTERPRETER pattern from design patterns, suggesting design patterns could serve architecturally under certain applications.
- Classification Based on Architectural Views: Enhances existing classifications with a focus on architectural views, intending to offer a more organized and accessible framework for understanding and applying patterns.

## Implementation and Audience
Content: The language incorporates and references well-documented patterns without repeating descriptions, focusing instead on explicating the connections between patterns.

Target Audience: Aimed at architects familiar with these patterns, helping them grasp the integrated "big picture" of architectural design through the interrelated patterns framework.

## Classification Scheme
- Implementation and Inter-relationships: Patterns are classified based on their implementation within a view, focusing on the intricate relationships between patterns.
- Primary and Secondary Views: Patterns are primarily associated with one view but can be applicable in additional views based on system-wide pattern combinations.

## Types of Elements in Views
- Components and Connectors: Central to the classification, representing runtime computation/data-storage units and interaction mechanisms, respectively.
- Exclusion of Certain Views: Some views, like module views dealing with implementation modules or allocation views addressing software element distribution, are not included in the current scheme.

## Overview of the Pattern Language
This pattern language encompasses component and connector views, detailing established and classical architectural patterns from recognized sources like POSA and SEI, along with a selection from other significant works to bridge gaps in the classical frameworks. It aims to offer a structured understanding of architectural patterns and their interconnections.

## Pattern Views and Classifications
### [[Layered View]]
Focuses on decomposing complex systems into interacting layers.
Patterns: LAYERS, INDIRECTION LAYER (also known as “virtual machine”).

### Data Flow View
Concerned with sequential data processing or transformation.
Patterns: BATCH SEQUENTIAL, PIPES AND FILTERS.

### Data-centered View
Addresses access to a central data repository by multiple components.
Patterns: SHARED REPOSITORY, ACTIVE REPOSITORY (or “blackboard”), BLACKBOARD.

### Adaptation View
Deals with system adaptability during evolution.
Patterns: MICROKERNEL, REFLECTION, INTERCEPTOR.

### Language Extension View
Focuses on abstracting the computation infrastructure through system-specific languages.
Patterns: INTERPRETER, VIRTUAL MACHINE, RULE-BASED SYSTEM.

### User Interaction View
Shows components offering user interfaces and their runtime structure.
Patterns: MODEL-VIEW-CONTROLLER, PRESENTATION-ABSTRACTION-CONTROL, C2.

### Component Interaction View
Highlights autonomous components exchanging messages.
Patterns: EXPLICIT INVOCATION, IMPLICIT INVOCATION, CLIENT-SERVER, PEER-TO-PEER, PUBLISH-SUBSCRIBE.

### Distribution View
Tackles the distribution of components across networked environments.
Patterns: BROKER, REMOTE PROCEDURE CALLS, MESSAGE QUEUING.
