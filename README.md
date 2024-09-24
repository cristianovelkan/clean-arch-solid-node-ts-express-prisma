# SOLID e Clean Architecture Example Project

The acronym ***SOLID*** is a set of code design principles that aim to facilitate the maintenance and evolution of software. It was introduced by Robert C. Martin in 2000 and consists of five principles:

- **S** - Single Responsibility Principle 
- **O** - Open/Closed Principle
- **L** - Liskov Substitution Principle
- **I** - Interface Segregation Principle
- **D** - Dependency Inversion Principle

# Clean Architecture

***Clean Architecture*** is a set of practices and techniques that aim to facilitate software maintenance and evolution. It was introduced by [Robert C. Martin in 2012](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html) and is composed of four layers:

- **Domain** - The innermost layer, where the system's business rules are located. It must be completely agnostic in relation to any technology/infrastructure.
- **Use Cases** - The intermediate layer, which orchestrates the data flow between the domain layer and the infrastructure layer. Each use case is a user intention.
- **Infrastructure** - The third layer, where the concrete implementations of the interfaces defined in the domain layer are located. It is responsible for handling technology details and is the only layer that may depend on frameworks and libraries. This is where you will find repositories and *controllers*, for example.
- **External Interface** - The outermost layer, which we usually do not have access to. This is usually where the input and output devices are located, such as the user interface, database, web browsers, mobile applications, etc. In general, this is where the application clients, database, external APIs, etc. reside.
