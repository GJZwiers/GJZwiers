# Object-Oriented Programming
As programs grow, developers need ways to structure and organize the relationships and interactions between application components. One way of doing so is called **object-oriented programming** (OOP), where related data and behavior are wrapped in **objects** and **classes**.

_Objects_ are collections of data stored in **key-value pairs**. This means a value can be accessed by looking up its corresponding key. Keys can be strings or numbers depending on the language implementation.

_Classes_ are objects that hold a blueprint to make one or more **instances** of itself. Each instance has its own data and behaves independently of other instances of the same class.

## Common Concepts of Classes
Variables defined inside classes are called **fields**. Sometimes there is extra logic involved in getting or setting the value of a particular field, in which case it is called a **property** with a **getter** and/or a **setter**. Field and property are often used loosely when people talk about classes.

Functions as part of classes are called **methods**. In certain languages class methods can be prefixed with an **access modifier** which determines if that method can be called by other parts of the application. **Public** access means the method is callable from anywhere, while **Private** means it can only be called from other methods inside the class. **Protected** methods can be called from the inside of the class and from other classes that derive from it (For more information, see [Inheritance](interactiond.md)). 

Fields that hold constant values can often be marked with a **readonly** modifier.

Instances of a class are made using a special function called a **constructor**. 

## Defining a Class

TypeScript
```typescript
class Calculator {

}
```

Python
```python
class Calculator:
    pass
```

C#
```csharp
public class Calculator {

}
```

Rust
```rust
struct Calculator {

}

impl Calculator {

}
```
