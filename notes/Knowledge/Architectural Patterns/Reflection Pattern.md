# Reflection Pattern
[[Adaptation View]]

TODO: RAW: Pattern: Reflection
Software systems constantly evolve and change over the time, and unanticipated changes are
often required. It is hard to automatically cope with changes that are not foreseen.
In a REFLECTION architecture all structural and behavioral aspects of a system are stored into
meta-objects and separated from the application logic components. The latter can query the
former (that may have changed at any point of time) in order to execute their functionality. Thus
REFLECTION allows a system to be defined in a way that allows for coping with unforeseen
situations automatically
