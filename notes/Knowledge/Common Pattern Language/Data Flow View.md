# Data Flow View
- System Representation: Viewed as subsequent transformations on input data streams.
- Concerns Addressed:
  - Transformation elements (components with input/output ports).
  - Data stream carriers (connectors with data in/out roles).
  - Connections (attachments linking components and connectors).
  - Quality Attributes: Modifiability, reusability, integrability.

## Architectural Patterns:

### BATCH SEQUENTIAL:
- For simple sequential data processing.
- Involves overhead for starting batches and data transmission.

### PIPES AND FILTERS:
- Suitable for stream-oriented data flows.
- Allows incremental input-to-output stream transformations.
- Features forks/joins, feedback loops, and a linear pipeline variant.
- Emphasizes pipe connectors for data transfer flexibility.
- Constant data flow between filters, differing from batch's discrete steps.
- Pure form restricts data sharing to adjacent filters.

## Comparisons and Use Cases:

### PIPES AND FILTERS vs. BATCH SEQUENTIAL:
- Pipes and Filters offer flexibility and constant data flow, contrasting with Batch Sequential's discrete processing and lack of connectors abstraction.
- Alternative Patterns:
- Pure Pipes and Filters for non-adjacent task data sharing limitations.
  - More relaxed forms can integrate with data-centered architectures (e.g., SHARED REPOSITORY, ACTIVE REPOSITORY, BLACKBOARD) for broader data sharing.
  - Can facilitate communication between layers when data flow through layers is necessary.
