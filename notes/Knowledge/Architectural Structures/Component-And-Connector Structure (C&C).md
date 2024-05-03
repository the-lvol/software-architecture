# Component-And-Connector Structure (C&C)
An [[Architectural Structure]]

- Focuses on the runtime functionality of the system, answering "What does the system do?"
- Emphasizes the system's purpose, often initiating architectural design.
- Views software systems as comprising components (black-box units of functionality) and connectors (communication paths between components).
- Components are what and connectors are how

## Key Concepts
- Components: Define the functional behavior of system parts.
- Connectors: Outline control and data exchange between components, including aspects like protocols, state transitions, and concurrency.

## Documentation:
- Combines textual descriptions (e.g., component responsibilities) with diagrams to illustrate communication protocols and other relevant architectural details.

## Stakeholder Roles
Critical for architects, and developers, and informative for customers and end users regarding overall system runtime behavior.

## Elements and Relations:
- Component: A functional unit with defined behavioral responsibility.
- Connector: Facilitates communication between components, detailing control and data exchange methods.

Both components and connectors are considered primary elements, capable of exhibiting behavior. Connectors, for instance, may offer functionalities like buffering, data conversion, protocol adaptation, remote procedure calls, and networking.

## Protocols and Behavior:
Connectors define protocols that prescribe both incoming and outgoing operations, including their sequencing, distinguishing them from class interfaces which detail available operations without specifying call sequences.

## Some Useful [[Structure]]s
| [[Structure]] | Description |
| :---          | :---        |
| Service structure | The units here are services that interoperate with each other by service coordination mechanisms such as SOAP. Important to connect system develop anonymously and/or independently from each other (Caliing an API of another service) |
| Concurrency structure | This component-and-connector structure allows the architect to determine opportunities for parallelism and the locations where resource contention may occur. The components are arranged into logical threads; a logical thread is a sequence of computations that could be allocated to a separate physical thread later in the design process. The concurrency structure is used early in the design process to identify the requirements to manage the issues associated with concurrent execution |
