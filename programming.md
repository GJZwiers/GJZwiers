# Fundamentals - Programming

This page aims to provide a high-level overview of common programming concepts. It begins with a bit of theory on each and then it shows them in practice through examples.

### On this page
1. [Storing Data in Variables](#storing-data-in-variables)
2. [Repeating Actions with Loops](#repeating-actions-with-loops)
3. [Controlling Program Flow](#cointrolling-program-flow)
4. [Writing Functions for Reusable Behaviors](#writing-functions-for-reusable-behaviors)

## Storing Data in Variables

In programming, application data is stored in **variables**. Every variable has a _name_, a _type_, and a _value_. 

The name can be almost anything, although usually there are a few rules to follow and a couple of good practices to uphold. One good principle is simply to __say what you mean__ when naming variables. Programming is not like writing a novel, where you might choose words that are exceptionally beautiful, provocative and/or extravagant. When writing code we want to use names that are clear, concise and descriptive instead. This helps to provide clarity for both yourself and your fellow developers, both in the present and in the future.

_Types_ are needed for the computer to understand how to work with a particular variable. Some common data types you'll come across are integers (whole numbers), floating point numbers, strings of text, booleans (true or false values) and more complex objects such as lists. Types can be _static_ where the type of the variable is not permitted to change over the course of a program, whilst others have _dynamic_ types which can. 

<details>
    <summary>More info on static vs. dynamic</summary>

    Using static types tends to have small performance benefits because compilers need to allocate more computer memory for dynamic variables to account for their changing nature.
</details><br>

The _value_ of a variable is closely linked to its type. An integer value might be 2 or 1991. A string value might be 'Hello' or '2'. Notice something peculiar? Integers are written down as is but strings are surrounded with quotes. Now we have the integer value 2 and the string value '2'. Although the integer and the string have the same _value_ they do not have the same _type_. This can be of importance when working with numbers because computers cannot use strings in calculations right away.

When a value does not change, it is called a _constant_, as opposed to the _static_ unchanging type mentioned before. Constant values are often written in capitals to distinguish them from other numeric values.

Programming syntax has certain **keywords**. There words are reserved by the language for a certain task and cannot be used as a variable name. One example is the word _if_ which is reserved for applying program logic.


### Examples

Variable declarations tend to have the following structure:
```
name = value
```
A language often places a variable keyword such as `var` at the start of the declaration as well:
```
var name = value
```
When a variable name has more than one word, we cannot use spaces. Instead, we can glue the words together and write the first character of every word after the first in uppercase. This style is called camel case, supposedly because of how the uppercase characters protrude like the humps on a camel's back:

```
var nameInCamelCase = ...
```

Another common style for variable names is snake case, which uses underscores between the words:
```
var name_in_snake_case = ...
```

Let's look at how you shouldn't name a variable. Check out the code below, which declares a variable with name 'Jimmy' and value '5' and then prints the text 'Jimmy is 5 years old' to a console window, using the value of the variable.
```
var jimmy = 5;

console.log('Jimmy is : {1} years old', jimmy)
```

The problem here is that although Jimmy is five, five is not Jimmy. Five is Jimmy's age. Let's change that:
```
var jimmiesAge = 5;

console.log('Jimmy is : {1} years old', jimmiesAge)
```
This is better, however, imagine there's someone else that's five years old as well, but not named Jimmy. We could try this:
```
var jimmiesAge = 5;

console.log('Jimmy is : {1} years old', jimmiesAge);
console.log('Angie is : {1} years old', jimmiesAge);
```
From a functional perspective this works fine, but this approach gets confusing quite fast. both Jimmy and Angie have a shared attribute, which is their age.

```
var age = 5;

console.log('Jimmy is : {1} years old', age);
console.log('Angie is : {1} years old', age);
```


## Repeating Actions with Loops



```
var counter = 0;

counter = counter + 1;
counter = counter + 1;
counter = counter + 1;

print(counter)
```

```
var counter = 0;

for (var i = 0; i < 3; i++) {
    counter = counter + 1;
}

print(counter)
```

Let's use a shorthand operator for addition:

```
var counter = 0;

for (var i = 0; i < 3; i++) {
    counter += 1;
}

print(counter)
```


## Controlling Program Flow with Logic



## Writing Reusable Behaviors with Functions


