# Role-Based System Pattern
[[Language Extension View]]

TODO: RAW: Pattern: Rule-Based System
Logical problems are hard to express elegantly in imperative languages that are typically used in
INTERPRETERS and VIRTUAL MACHINES. Consider for instance an expert system that provides
the knowledge of an expert or a set of constraints. In imperative languages these are expressed
by nested if-statements or similar constructs which are rather hard to understand.
A RULE-BASED SYSTEM offers an alternative for expressing such problems in a system. It
consists mainly of three things: facts, rules, and an engine that acts on them. Rules represent
knowledge in form of a condition and associated actions. Facts represent data. A RULE-BASED
SYSTEM applies its rules to the known facts. The actions of a rule might assert new facts, which,
in turn, trigger other rules.

