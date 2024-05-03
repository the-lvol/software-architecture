# Presentation-Abstraction-Control Pattern
[[User Interaction View]]

TODO: RAW: Pattern: Presentation-Abstraction-Control
An interactive system may offer multiple diverse functionalities that need to be presented to the
user through a coherent user interface. The various functionalities may require their own custom
user interface, and they need to communicate with other functionalities in order to achieve a
greater goal. The users need not perceive this diversity but should interact with a simple and
consistent interface.
The system is decomposed into a tree-like hierarchy of agents: the leaves of the tree are agents
that are responsible for specific functionalities, usually assigned to a specific user interface; at
the middle layers there are agents that combine the functionalities of related lower-level agents
to offer greater services; at the top of the tree, there is only one agent that orchestrates the
middle-layer agents to offer the collective functionality. Each agent is comprised of three parts:
a Presentation takes care of the user interface; an Abstraction maintains application data and the
logic that modifies it; a Control intermediates between the Presentation and the Abstraction and
handles all communication with the Controls of other Agents.

