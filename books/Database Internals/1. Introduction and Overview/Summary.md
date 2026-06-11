A database is a collection of subsystems where each subsystem selects different tradeoffs to optimise for different workloads and requirements.  
A database consists of the storage engine subsystem with various components built on top such as the execution engine and query processor all of which have their own components.  
- Query processor must parse and validate the query and then optimize it to create execution plans
- Execution engine takes the query plan and executes the steps
- Storage engine ensures data is written safely without affecting others
Memory-based databases are faster than databases that require disk based I/O and they're also easier to work with because they have greater flexibility in the number of data structures and optimisations they can utilise, with the tradeoff being potential loss of some state despite best efforts with implementing persistence.  
A database can be classified in many ways typically as row vs column storage. It's important to understand your requirements to choose the correct database otherwise performance and costs may suffer.  
A database is described as a logical and modular system of component when in reality implementation may couple components for optimization purposes.  
Databases tend to store data separately from indexes, as different files, where data files may take different forms but typically be stored per table.  
Storage engines tend to differ in how they handle avoidable in-memory data buffering, whether they record updates or use immutable approaches and how they handle data ordering.  