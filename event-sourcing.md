# Joys Of Event Sourcing NodeJS

decade of experience - [https://www.youtube.com/watch?v=LDW0QWie21s&feature=youtu.be&t=2391](https://www.youtube.com/watch?v=LDW0QWie21s&feature=youtu.be&t=2391)

why not to use it - [https://chriskiehl.com/article/event-sourcing-is-hard](https://chriskiehl.com/article/event-sourcing-is-hard)

how it's awesome - message-db (eventide project + nodejs) and easy to get started

success cases - [https://martinfowler.com/articles/lmax.html](https://martinfowler.com/articles/lmax.html)

What it is:

- Check out my presentation on the subject with paired github repo
- presentation - [https://gitpitch.com/wolfejw86/talks-nodejs-event-sourcing#/1](https://gitpitch.com/wolfejw86/talks-nodejs-event-sourcing#/1)
- [https://github.com/wolfejw86/message-db-client](https://github.com/wolfejw86/message-db-client)

What it isn't and what's hard:

- UX can be forced to play along in certain situations - task based intead of update based
- not getting bounded contexts right for the business domain - causing heavy change / flux in event contracts - causing loss of fidelity
- spaghetti contracts where "who's reading what from what stream" becomes unclear
- materialization / projection will become expensive - snapshotting is a must

Use Cases: 

- microservices
- domain driven design - domain / ubiquitous language makes life easier
- scaling concerns

Donts:

- single db for all services
- single db for each service - can work but tricky

Do:

- use streams - think kafka - however kafka has poor support for optimistic concurrency control
- use event driven architecture
- can start with a single server and scale out without complex deployment
- Event storm your system
    - talk through domain
    - find bounded contexts
    - find major concepts

Keywords:

- **events - data + event type (think polymorphism) usually stored in order**
- **streams - collections of events**
- **event store - database - build your own or use product**
- **projections - processes a stream into an aggregate entity - can be stored as a read model**
- **read model -** might not be necessary - especially if aggregate streams are less than 100 events
- **event sourcing -** how to handle data in distributed systems in a scalable way - storing everything as events means everything in the domain logic is a first class citizen

Why this way is extra good:

- linearization of messages - ensures easy consistency
- Also theres all sorts of race conditions/problems of publishing/reading out of order or events being consumed before the proper readers have got to it.

Next steps:

- process managers
- actor model

Further Reading:

- the dark side of event sourcing -

[https://www.movereem.nl/files/2017SANER-eventsourcing.pdf](https://www.movereem.nl/files/2017SANER-eventsourcing.pdf)

- aggregate design pt1,2,3 - [https://dddcommunity.org/library/vernon_2011/](https://dddcommunity.org/library/vernon_2011/) pt1 - [https://dddcommunity.org/wp-content/uploads/files/pdf_articles/Vernon_2011_1.pdf](https://dddcommunity.org/wp-content/uploads/files/pdf_articles/Vernon_2011_1.pdf)
- versioning in event sourced system [https://leanpub.com/esversioning](https://leanpub.com/esversioning) - don't version - refactor with a copy + transform technique
- azure event sourcing handbook - [http://download.microsoft.com/download/e/a/8/ea8c6e1f-01d8-43ba-992b-35cfcaa4fae3/cqrs_journey_guide.pdf](http://download.microsoft.com/download/e/a/8/ea8c6e1f-01d8-43ba-992b-35cfcaa4fae3/cqrs_journey_guide.pdf)

Other Good Talks:

- [https://www.youtube.com/watch?v=GzrZworHpIk](https://www.youtube.com/watch?v=GzrZworHpIk)
