# Law Of Demeter
Informal definition

    For all classes C, and for all methods M attached to C, all objects to which M sends a message must be instances of classes associated with the following classes: The argument classes of M (including C). The instance variable classes of C. (Objects created by M, or by functions or methods which M calls, and objects in global variables, are considered arguments of M.) 

