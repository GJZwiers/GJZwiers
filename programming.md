# Fundamentals - 1

This page aims to provide a high-level overview of common programming concepts. It begins with a bit of theory on each and then it shows them in practice through examples.

### On this page
1. [Storing Data in Variables](#variables)
2. [Repeating Actions with Loops](#loops)
3. [Controlling Program Flow](#flow-control)
4. [Writing Functions for Reusable Behaviors](#functions)

## Storing Data in Variables

In programming, application data is stored in **variables**. Every variable has a _name_, a _type_, and a _value_. 

The name can be almost anything, although there are usually a few rules to follow and a couple of good practices to uphold. One good principle is simply to __say what you mean__ when naming variables. Programming is not like writing a novel, where you might choose words that are exceptionally beautiful, provocative and/or extravagant. When writing code we want to use names that are clear, concise and descriptive instead. This helps to provide clarity for both yourself and your fellow developers, both in the present and in the future.

_Types_ are needed for the computer to understand how to work with a particular variable. Some common data types you'll come across are integers (whole numbers), floating point numbers, strings of text, booleans (true or false values) and more complex objects such as lists. Types can be _static_ where the type of the variable is not permitted to change over the course of a program, whilst others have _dynamic_ types which can. 

<details>
    <summary>More info on static vs. dynamic</summary>

    Using static types tends to have small performance benefits because compilers need to allocate more computer memory for dynamic variables to account for their changing nature.
</details><br>

The _value_ of a variable is closely linked to its type. An integer value might be 2 or 1991. A string value might be 'Hello' or '2'. Notice something peculiar? Integers are written down as is but strings are surrounded with quotes. Now we have the integer value 2 and the string value '2'. Although the integer and the string have the same _value_ they do not have the same _type_. This can be of importance when working with numbers because computers cannot use strings in calculations right away.

When a value does not change, it is called a _constant_, as opposed to the _static_ unchanging type mentioned before. Constant values are often written in capitals to distinguish them from other numeric values.

Programming syntax has certain **keywords**. There words are reserved by the language for a certain task and cannot be used as a variable name.


### Examples



```
var jimmy = 5;

print('Jimmy is : ', jimmy)

```
```
var age = 5;

print('Jimmy's age is: ', age)

```

## Loops

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


## Repeating Actions with Loops



## Controlling Program Flow



## Writing Reusable Behaviors with Functions