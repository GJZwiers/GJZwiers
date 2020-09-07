# Object-Oriented Programming
As programs grow, developers need ways to structure and organize the relationships and interactions between application components. One way of doing so is called **object-oriented programming** (OOP), where related data and behavior are wrapped in **classes**.

_Classes_ are objects that store a blueprint to make one or more **instances**. Each instance has its own data and behaves independently of other instances of the same class.

## Common Concepts of Classes
Variables defined inside classes are called **fields**. Sometimes there is extra logic involved in getting or setting the value of a particular field, in which case it is called a **property** with a **getter** and/or a **setter**. Field and property are often used loosely when people talk about classes.

Functions as part of classes are called **methods**. In certain languages class methods can be prefixed with an **access modifier** which determines if that method can be called by other parts of the application. **Public** access means the method is callable from anywhere, while **Private** means it can only be called from other methods inside the class. **Protected** methods can be called from the inside of the class and from other classes that derive from it (For more information, see [Inheritance](interactiond.md)). 

Fields that hold constant values can often be marked with a **readonly** modifier.


### Samples - Defining a Class

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

Rust*
```rust
struct Calculator {

}

impl Calculator {

}
```
##### * Rust separates classes into `struct`ures and `impl`ementations. This is related to advanced OOP topics which are explained in more detail in [Creating Abstractions](interactions.md).

## Initialization
An instance of a class is initialized with a special method called a **constructor**. This method can take input parameters that are used to set the starting state of that instance.

TypeScript
```typescript
class Calculator {

    constructor() {

    }
}
```

Python
```python
class Calculator:

    __init__():
        pass
```

C#
```csharp
public class Calculator {

    public Calculator() {

    }
}
```

Rust*
```rust
struct Calculator {

}

impl Calculator {
    pub fn new() -> Calculator {
        
    }
}
```