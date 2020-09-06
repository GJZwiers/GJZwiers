# Working with Different Types of Data


## Booleans

True or not true? That's exactly what boolean values are about: a value that is either `true` or `false`.

## Strings

## Numbers

## Arrays, Enums and Tuples

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
