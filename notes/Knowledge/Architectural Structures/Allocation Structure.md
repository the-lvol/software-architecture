# Allocation Structure
An [[Architectural Structure]]

- Addresses the mapping of software elements (especially from the [[Component-And-Connector Structure (C&C)]]) to hardware platform elements.
- Focuses on software requirements (e.g., processing power, memory, network bandwidth) and hardware provisions.

## Stakeholder Roles
Relevant to
- Maintainers: For deployment and maintenance.
- Users/Customers: Understanding how functionality correlates with hardware.
- Developers: Implementing the system based on hardware constraints.
- Architects: Designing the system with hardware considerations in mind.

## Elements and Relations
- Software Elements: Includes executables or link libraries that contain components from the C&C viewpoint.
- Environmental Elements: Refers to computing hardware nodes where the software will run.

## Key Relations
- Allocated-to Relations: Indicates the assignment of software elements to hardware at runtime, which can be static or dynamic (e.g., components moving between hardware nodes).
- Software Dependencies: Interdependencies among software elements.
- Protocol Links: Communication protocols used among hardware nodes, detailing how environmental elements interact.

This viewpoint essentially bridges the gap between the abstract design of a software system (as seen in the [[Component-And-Connector Structure (C&C)]]) and the concrete hardware environment it will operate in, highlighting the importance of understanding both software needs and hardware capabilities for effective system deployment and operation.

## Some Useful [[Structure]]s
| [[Structure]] | Description |
| :---          | :---        |
| Deployment structure | The deployment structure shows how software is assigned to hardware processing and communication elements. It helps reason about performance, data integrity, security, and availability by showing how software components are mapped to physical hardware elements like processors and communication channels. It's particularly useful for distributed and parallel systems |
| Implementation structure | This structure shows how software elements (usually modules) are mapped to the file structure(s) in the system’s development, integration, or configuration control environments. This is crucial for managing development activities and build processes by mapping software elements (usually modules) to the file system organization within the development, integration, or configuration control environments. |
| Work assignment structure | This structure assigns responsibility for implementing and integrating the modules to the teams who will carry it out. It clarifies the architectural and management implications of assigning development and integration tasks to specific teams. It considers the expertise required by each team and helps ensure functional cohesion by assigning units of common functionality to single teams. |

