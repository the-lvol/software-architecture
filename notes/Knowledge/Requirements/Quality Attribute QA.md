# Quality Attribute QA
    A quality attribute (QA) is a measurable or testable property of a system that is used to indicate how well the system satisfies the needs of its stakeholders. You can think of a quality attribute as measuring the "goodness" of a product along some dimension of interest to a stakeholder

- Quality attributes are characteristics of a system beyond its core functionality
- They describe how well the system meets various non-functional requirements (NOTE, we're trying not to use the term non-functional requirements due to pollution of the term).
- Examples include performance, security, availability, and usability.
- They are not independent: achieving one quality attribute may impact others.
- There are challenges in defining, measuring, and reasoning about quality attributes.

## Architect's Perspective
- Architects need to consider quality attributes when making design decisions.
- They should use quality attribute scenarios to characterize desired behavior.
- Different quality attribute communities use different vocabulary, which can be confusing.
Two Categories of Quality Attributes

**Runtime qualities**: Describe how the system behaves during operation (e.g., performance, availability).

**Development qualities**: Describe how the system is built and maintained (e.g., modifiability, testability).
Trade-offs are Necessary

It is often impossible to achieve all quality attributes perfectly. Architects need to make trade-offs to satisfy the most important requirements.

## Requirements Specification
Note, that the disadvantage of enforcing these requirements is that sometimes force-fits have to be done, but the advantage is that an emphasis on commonalities is used

### Quality Attribute Characteristics
1. Stimulus: An event that triggers the system, varying across communities (e.g., performance, usability, security) and includes development actions like modification requests or development phase completion.
2. Stimulus Source: The origin of the stimulus, influencing system treatment based on the source's trust level, e.g. trusted vs. untrusted user.
3. Response: Defined actions the system or developers must take in reaction to the stimulus, tailored to the specific quality attribute scenario (e.g., processing events, implementing modifications).
4. Response Measure: Metrics to evaluate if the system's response meets the requirement, varying by attribute (e.g., latency for performance, time for modifiability).

Additional characteristics

5. Environment: The scenario's context, affecting stimulus treatment (e.g., code modification received after release code freeze, how many times have said component failed?).
6. Artifact: The specific system part affected by the requirement, possibly targeting entire systems or specific components (failure in data store vs. metadata store).

![[Six-Part Scenario]]

### Process of Specification:
To effectively apply quality attribute scenarios to a system, general scenarios must be customized into concrete scenarios. This involves adjusting the generic scenarios to fit the unique context and requirements of the system in question
