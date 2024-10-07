# Task
## Input Data:

A CRM system for a telecommunications company with 100 operators.

### CRM consists of:

- Clients (individuals and legal entities)
- Orders (service orders provided to the client)
- Tickets (support requests)
- Task Manager (Kanban board for handling tickets, includes boards, tasks, and a dashboard with dynamic filters)

### WorkFlow:

- The user logs in to the CRM:
o User profile
o User notifications

- The user can access clients:
o View client list
o Search by client name
o Edit client details
o Create a new client

- The user can access orders:
o View order list for clients
o View order list
o Search for an order
o Create an order for a client

- The user can access tickets:
o View tickets
o Create a ticket for a client
o Close a ticket

- The user can access the task manager:
o A board is created for the user
o When a ticket is created, a task is added to the board
o The task follows a business process
o Once the task is complete, the ticket is automatically closed, and notifications are sent (to the manager and client)
o Integration with external systems (incoming/outgoing)

- The Task Manager includes:

o A dashboard displaying task information
o Dynamic filters
o Response time of less than 1 second

- System Requirements:

o High availability 
o High load capacity (500 requests per second)

### Problems to Solve:

1. Develop a domain model (any notation)
2. Create a unified architecture (monolith, SOA, MSA) with justification for the chosen approach
3. Prepare an optimal integration solution
4. Choose a fault tolerance and load-handling approach
5. Create a block diagram/architecture diagram, possibly in phases (Day 0-Day 2)
6. Select languages and technology stack with an alternative solution. Provide a comparative evaluation table with preferences for the top 1-2 main technologies.
7. Assess technical infrastructure, computing, RAM, long-term storage, and network for a 5-year operation period
8. Optional: Evaluate overall solution effort (development roles and person-months)

### Reporting Documents:

1. Documents should contain the following diagrams:

o Use Case, 
o ERD, 
o DFD, 
o Sequence Diagrams (general and detailed), 
o Class Diagrams, 
o Component Diagram, 
o Deployment Diagram, 
o Integration Diagram, 
o DB Architecture.
2. Prepare API documentation (Swagger)
3. Present the results in two documents:
o A document with diagrams, tables, and comments
o A presentation on key diagrams and ideas.

### Additional
Legacy components (Clients and Orders) use an older stack. Try to integrate these legacy systems into the new architecture.



