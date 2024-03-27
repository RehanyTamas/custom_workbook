#Custom Workbook

##UiPath

###What is RPA?
-Robotic Process Automation (RPA) refers to the use of software robots or "bots" to automate repetitive, rule-based tasks within business processes.
-These tasks are typically manual, time-consuming, and prone to human error
-RPA robots mimic human interactions with software applications and systems by interacting with user interfaces, manipulating data, and executing predefined actions.

###What is UiPath?
-UiPath is one of the leading providers of Robotic Process Automation (RPA) software, offering a platform for automating repetitive, rule-based tasks.
-Low-code (Visual, drag-and-drop approach, wide range of pre-built activities.)

###What are the differences between attended and unattended robots?
-Attended robots work alongside human employees, assisting them with tasks in real-time.
-These typically require user interaction.
-Unattended robots operate autonomously, executing tasks without human intervention.

###What are selectors?
-They are used to identify UI elements within applications or web pages.
-For this pupose they can use various elements, such as id, name, class, tag, parentid.
-There are also dynamic sleectors, which can be used to refer to elements, which's tes change on refresh. (Syntax: *)

###Explain data scraping in UiPath?
-Data scraping in UiPath involves extracting data from websites or web applications.
-UiPath automatically creates selectors to locate similar data elements on web pages, enabling the extraction of tables, lists íand other strucured data.

###What is low-code?
-Low-code development refers to a software development approach that allows developers to create applications with minimal hand-coding.
-Typically through a visual interface or configuration rather than traditional programming.
-The goal of low-code platforms is to enable rapid application development and streamline the development process.

##CQRS

###What is CQRS, and what problem does it address in software architecture?
-CQRS stands for Command Query Responsibility Segregation.
-It is an architectural pattern that separates read and write operations (commands and queries) into two distinct paths.

###Explain the concept of commands and queries in the context of CQRS.
-Commands: Actions that change the state of the system (e.g., creating a new record, updating an existing record).
-Queries represent requests for data retrieval or querying existing state.

###What are the benefits of using CQRS in software development?
-Improved scalability (independent scaling of read and write operations)
-Better performance optimization (diferent optimization for the two sides)
-Enhanced flexibility in handling complex domain logic (commands can encapsulate complex business rules and workflows without being constrained by the requirements of read operations.)
-Improved maintainability (due to the distinct models and logic, changes or updates to one path are less likely to impact the other)

###Discuss the challenges and trade-offs associated with implementing CQRS in a software project.
-Implementing CQRS introduces complexities such as maintaining consistency between read and write models.
-Managing eventual consistency, and ensuring synchronization between command and query paths.

###What is event sourcing in CQRS?
-Event sourcing involves capturing all changes to the application state as a sequence of events.
-These events represent facts or immutable records of what has happened in the system.
-These events are then stored and can be replayed to rebuild the application state.
-Event sourcing enables a complete audit trail of system state changes.
-CQRS complements event sourcing by providing separate read and write models that can be optimized independently.

###What factors should be considered when deciding whether to adopt CQRS in a software project?
-Complexity of domain logic: Applications with complex domain logic that may benefit from a clearer separation of write and read concerns.
-Scalability requirements:Applications with varying workloads.
-Performance requirements: Applications with demanding performance requirements, especially for read-heavy workload.
-Development team experience: Adopting CQRS requires a solid understanding of the underlying principles and best practices.

###Specific use cases or domains where CQRS is well-suited include?
-Financial systems: Financial transactions often have complex business rules and scalability requirements that align well with CQRS (Bonus points for event sourcing).
-Analytics and reporting: Systems requiring real-time or near-real-time access to large volumes of data.
-Collaboration platforms: Complex concurrency requirements that can be addressed using CQRS.