# Requirement
TODO: definition

## Two Types Of Descriptions Of Architecturally Significant Requirements
The primary goal is to facilitate the creation of "test cases" to compare and evaluate different architectural designs. This approach ensures designs meet both functional and non-functional requirements, balancing critical quality attributes against each other.

### Scenario-Based
Focuses on a subset of overall scenarios that detail the functional requirements of the system. These scenarios can be augmented with additional requirements like performance, availability, and reliability.

### Quality Attribute-Based
Complements scenario-based requirements by identifying critical quality attributes (e.g., modifiability, performance) the system must fulfill. It's noted that these attributes often conflict, necessitating prioritization.

### Example
In the NextGen POS case, a scenario is a specific path through a use case. An example of such a scenario is:

    Process Sale: A customer arrives at a checkout with items to purchase. The cashier uses the POS system to record each purchased item. The system presents a running total and line-item details. The customer enters payment information, which the system validates and records. The system updates inventory. The customer receives a receipt from the system and then leaves with the items.

Critical architectural attributes for the NextGen POS system are:
- Availability. The system shall be highly available since the effectiveness of sales depends on its availability
- Portability. The system shall be portable to a range of different platforms to support a product line of POS systems
- Usability. The system shall be usable by clerks with a minimum of training and with a high degree of efficiency

## Types And Responses

### Types
1. Functional Requirements (see [[Functionality]]): Define core tasks the system must perform (what the system does).
2. [[Quality Attribute QA]] Requirements: Specify how well functions should be done (speed, error handling, deployment time, cost limits).
3. Constraints: Predetermined design choices, often stemming from external factors (ex: must use an existing module).

### Responses
1. Functional Requirements (see [[Functionality]]): Assign responsibilities through the design.
2. [[Quality Attribute QA]] Requirements: Creates structures, behaviors, and interactions between elements to meet quality goals.
3. Constraints: Satisfied by accepting the design decision and reconciling it 
with other affected design decisions.
