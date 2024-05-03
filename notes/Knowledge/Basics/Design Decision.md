# Design Decision
    TODO

## 7 Categories
- Not the only way of categorizing
- Some may overlap, okay if a decision is in two categories
- There to ensure that every important decision is considered
- TODO: I have seen these before, but not sure where

### Allocation Of Responsibilities
- Identification of Responsibilities:
  - Fundamental system functions.
  - Architectural infrastructure components.
  - Satisfaction of [[Quality Attribute QA]] (plural).
- Allocation to Elements:
  - Non-runtime elements: Modules (see [[Module Decomposition Structure]]).
  - Runtime elements: Components, Connectors (see [[Component-And-Connector Structure (C&C)]]).
- Decision Strategies:
  - Functional Decomposition: Breaking down complex systems into simpler, functional components. (See [[Functionality]])
  - Real-World Modeling: Aligning system components with real-world entities.
  - System Operation Modes: Grouping based on the system's operational phases.
  - Quality Requirements Grouping: Organizing elements based on similar QAs like processing speed, security levels, and adaptability to changes.

### Coordination Model
Coordination Model Definition: A framework of mechanisms through which system elements interact and coordinate.

Decisions in Developing a Coordination Model:
1. Element Identification:
  - Which system elements need to coordinate?
  - Restrictions on coordination between certain elements.
2. Properties of Coordination:
   - Timeliness: How promptly elements interact.
   - Currency: The relevance of the information exchanged.
   - Completeness: The extent of information exchange.
   - Correctness: Accuracy of the exchanged information.
   - Consistency: Uniformity of the information across interactions.
3. Communication Mechanisms:
   - Selection based on the above properties.
   - Types:
     - Stateful vs. Stateless: Whether interactions remember past exchanges.
     - Synchronous vs. Asynchronous: Timing of response relative to request.
     - Guaranteed vs. Nonguaranteed Delivery: Reliability of message delivery.
     - Performance Properties: Throughput and latency considerations.

Objective:
- To design a coordination model that ensures effective and efficient interaction among system components, aligning with specific requirements on timeliness, reliability, and performance.

Application:
- Critical for ensuring system components work together harmoniously, supporting the overall goals of the software architecture in terms of functionality, reliability, and scalability.

### Data Model
- Major Data Abstractions & Operations:
  - Creation, initialization, access, persistence, manipulation, translation, and destruction of data items.
- Metadata Compilation:
  - Ensuring consistent interpretation of data.
- Data Organization:
  - Storage options: Relational databases, object collections, or both.
  - Data mapping strategies between different storage forms.

### Management Of Resources
- Resource Identification and Limits:
  - Hard resources (CPU, memory, hardware buffers) and soft resources (locks, thread pools).
- Resource Management and Sharing:
  - Which elements manage resources and strategies for contention arbitration?
- Saturation Impact:
  - Different effects on performance due to resource load, e.g., CPU load vs. memory scarcity.

### Mapping Among Architectural Elements
- Modules and Runtime Elements:
  - Mapping from modules ([[Module Decomposition Structure]]) to each other
  - Creation and code containment relationships.
- Runtime Elements to Processors:
  - Assignment for execution.
- Data Model Items to Data Stores:
  - Allocation of data to specific storage.
- Delivery Units Mapping:
  - Modules and runtime elements to deliver packages.

### Binding Time Decisions
1. Variation Scope and Timing:
   - Decisions range from developer-made design time choices to end-user-driven runtime adjustments.
2. Examples:
   - Allocation of Responsibilities: Build-time module selection through parameterized makefiles.
   - Coordination Model: Runtime negotiation of communication protocols.
   - Resource Management: Runtime acceptance and driver installation for new peripheral devices.
   - Technology Choices: Dynamic app downloads tailored to the user's device specifications.
3. Cost Considerations:
- Balancing the costs of initial decision implementation against the costs and feasibility of later modifications.
- Strategies to mitigate impacts of platform changes or technology shifts, weighing early vs. late binding costs.

Objective:
To facilitate flexibility and adaptability in system design and operation, allowing for variations in configuration and functionality at different stages of the lifecycle, while carefully managing the associated costs and trade-offs.

### Choice Of Technology
Role: Technology choices are crucial in realizing architectural decisions, which may be predefined by constraints or require selection by the architect.
Decision Factors:

1. Technology Availability:
Identifying technologies capable of fulfilling architectural requirements across all decision categories.

2. Development Support:
Evaluating the adequacy of tools (IDEs, simulators, testing platforms) for the chosen technology.

3. Knowledge and Support:
Assessing internal expertise and external resources (e.g., training, consulting availability) to ensure successful implementation.

4. Technology Implications:
Considering how a technology choice might dictate or limit options in coordination models, resource management, and other architectural aspects.

5. Compatibility with Existing Systems:
Ensuring new technologies integrate with and operate alongside, the current technology stack, including communication, monitoring, and management capabilities.

6. Objective:
To select technologies that not only align with architectural visions but also support development, integration, and future scalability, balancing innovation with practical considerations of support, compatibility, and side effects.
