# Using Lists and Objects

> In this guide you will learn about store and organize collections of data.

## Lists
Programming languages offer ways to store lists of values. Across languages, three kinds of list types are often available:
* `Static arrays` have a fixed number of elements of the same type
* `Enums` contain a group of distinct values
* `Array lists`, also called `dynamic arrays` or `vectors` hold a variable number of elements and types

Each element in a list has an **index** that can be used to access its value.

## Objects

_Objects_ are collections of data stored in **key-value pairs**. This means a value can be accessed by looking up its corresponding key. Object keys can be strings or numbers depending on the language.

There are generally two ways to get a value from an object. The first is called **dot notation** where the name of the variable is typed that has stored said object and follow it with a dot and the name of the key that holds the value. The second is string index notation where the name of the object variable is followed with square brackets including the name of the key as a String e.g. `["key"]`

The following samples show how an object literal is declared and how a value `"John"` can be accessed by its corresponding key `firstName`.

### Samples -  Object Declaration and Access

JavaScript
```javascript
let person = { 
    firstName: "John",
    lastName: "Smith" 
};

console.log(person["firstName"], person["lastName"]);
```

Python
```python
person = { 
    "firstName": "John",
    "lastName": "Smith" 
}

print(person["firstName"], person["lastName"])
```

C#
```csharp
var person = new { 
    firstName = "John",
    lastName = "Smith"
};

Console.WriteLine(person.firstName, person.lastName);
```

Rust
```rust
struct Person {
    firstName: &str,
    lastName: &str
}

let firstName = "John";
let lastName = "Smith";

let person = Person { firstName, lastName };

println!("{}, {}", person.firstName, person.lastName);
```




## Value Types versus Reference Types

An important thing to keep in mind when using different data types is how they are handled in computer memory and the way it affects their behavior. Programs store data from variables in two places. Primitive values such as integers and booleans are placed on the **stack**, which is somewhat like a stack of papers where each sheet holds the information about the value. When a new variable is declared it is added on top of the stack. When a value is no longer needed, it is taken out.  
On the other hand, complex types like arrays and objects are stored on the **heap**, while only a **pointer** to that location in memory is stored on the stack. This more indirect approach has the benefit of keeping the stack work fast. When a new variable is assigned the value of an existing object a new pointer or _reference_ is placed on the stack, pointing to the _same_ value on the heap.

```javascript
let firstObject = {
    luckyNumber: 7,
    randomNumber: 5
};

let secondObject = firstObject;

firstObject.luckyNumber = 3;
console.log(secondObject.luckyNumber);
```
Here we declare an object with two properties and then assign another variable to the object. Next, we change the value of the property `luckyNumber`.

What value is printed to the console for `secondObject.luckyNumber`?
* 7
* 3
* 5

