# Experimental Prototyping
Used to gauge the adequacy of a proposed architecture, or details hereof, before investing in a large-scale implementation of it. Experimental prototypes are typically used to measure software architecture qualities; e.g., to make quantitative measurements of performance or portability

- **Purpose**: Measure specific aspects of a proposed architecture or details thereof, before the development of the target system.
- **Main Users**: Primarily architects, to prove that the system can meet qualitative requirements like performance, availability, or portability.
- **Context of Use**:
  - Establish experimentally if the proposed architecture meets qualitative requirements. Simulate the intended deployment environment to evaluate architecture under execution conditions.
- **Challenges**:
  - Validity of measurements for architectural qualities before full system build and deployment.
  - Importance of starting evaluation of critical qualities, like performance, early in the development phase.
- **Applications**:
  - **Overall Level**: Assess core software qualities (e.g., performance vs. modifiability trade-offs in the 'Closed-Loop Process Control' case).
  - **Intermediate Level**: Quantitatively measure how well an architecture fulfills requirements (e.g., modifiability and reusability through components and connectors).
  - **Detailed Level**: Test the use of architectural/design patterns on overall architectural qualities (e.g., balance between modifiability and performance).

- **Key Insights**:
  - Experimental prototyping helps discover solutions to balance trade-offs between different architectural qualities.
  - Can demonstrate through real code how a certain architecture addresses or fails to address key requirements.
  - Helps in understanding and settling the basic tension in the use of patterns regarding non-runtime and runtime qualities (e.g., modifiability vs. performance).
