# Design Principles
Design Principles mini course from manuelzapata.com

## A single reason
### Single Responsability (SRP)
- A component will have a single reason to change
- Module -> A module can be seen as an Implementation Unit
- Understand what are the class responsabilities 

## Extend, Do not Modify
### Open Close Principle (OCP)
- A module can be, Open to be extended, Close to be modified
- Add new functionalities without too many changes on code
- All attributes of a class should be private
- Global variables brake this principle
- See Decorator, Strategy, Factory patterns

## Like father like son
### Liskov substitution (LSP)
- You should be able to replace the Son Instance by the father Instance, and the programm should remain working
- Tis principle will be broken when:
  - The Son Class modify the behavior of the Father Class
  - Override a method of the Father Class and do not write code
  - When the Son Class throw exceptions that Father Class can not handle
  - When the Son Class make incompatible one or more methods of the Father Class

## Do not depend on what you do not need
### Interface Segregration (ISP)
- Clients should not depend on unutilised methods
- Intefaces should not have methods that we do not need

## Abstraction is good too
### Dependency Inversion (ISP)
- High level modules should depend on abstractions
- Abstractions should not depend on details
