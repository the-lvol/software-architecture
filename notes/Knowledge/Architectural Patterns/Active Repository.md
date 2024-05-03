# Active Repository
[[Data Centered View]]

TODO: RAW: Pattern: Active Repository
A system needs to have a SHARED REPOSITORY, but it should not just be passively accessed
by accessor components. Clients need to be immediately informed of specific events in the
shared repository, such as changes of data or access of data. “Polling” (i.e. querying in frequent
intervals) the SHARED REPOSITORY for such events does not work, for instance, because this
does not deliver timely information or inflicts overhead on the system performance. An ACTIVE REPOSITORY is a SHARED REPOSITORY that is “active” in the sense that it informs
a number of subscribers of specific events that happen in the shared repository. The ACTIVE
REPOSITORY maintains a registry of clients and informs them through appropriate notification
mechanisms.
