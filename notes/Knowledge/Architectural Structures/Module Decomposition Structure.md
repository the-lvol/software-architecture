# Module Decomposition Structure
An [[Architectural Structure]]

Each module is assigned specific computational responsibilities and is the basis of work assignments for a team (frontend team, database team, etc.)

In large projects each module can be assigned to subteams (imagine having to create an ERP system as the backend, that requires more than 1 team)

An example would be a class diagram in object-oriented designs

The structure is static because it focuses on how the system's functionality is divided up, and how it can be assigned to teams

## Stakeholders
Architects and developers working on or with the system

## Elements And Relations

### Elements
- Class: Describes object properties existing at runtime.
- Package: Logical division of classes, akin to Java packages or a conceptual grouping of system classes.
- Interface: Defines the interface a class realizes, applicable to both programming languages like Java and conceptual class interfaces.

### Relations
- Association: Indicates a strong or weak aggregation relationship, applicable between classes.
- Generalization: Represents a generalization relation, usable between classes or interfaces.
- Realization: Highlights that one element realizes another, typically from a class to an interface it implements.
- Dependency: Denotes a dependency relationship, applicable across all elements.

## Some Useful [[Structure]]s
| [[Structure]] | Description |
| :---      | :---        |
| Decomposition | The units are modules that are related to each other by the is-a-submodule-of relation. This structure is often used as the basis for the development project's organization. |
| Uses | The units are also modules, perhaps classes. The units are related by the uses relation, a specialized form of dependency: A unit of software uses another if the correctness of the first requires the presence of a correctly functioning version (as opposed to a stub) of the second. This structure is used to engineer systems that can be extended to add functionality. |
| Layer | The modules in this structure are called layers. A layer is an abstract “virtual machine” that provides a cohesive set of services through a managed interface. This structure is used to imbue a system with portability. |
| Class (or generalization) |The module units in this structure are called classes. The relation is inherits from or is an instance of. This view supports reasoning about collections of similar behavior or capability. |
| Data model | The data model describes the static information structure in terms of data entities and their relationships. For example, in a banking system, entities will typically include Account, Customer, and Loan. Account has several attributes, such as account number, type (savings or checking), status, and current balance. A relationship may dictate that one customer can have one or more accounts, and one account is associated to one or two customers |
