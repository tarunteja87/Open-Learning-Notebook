# Python OOPS
- Introduction to OOPS

## Introduction to Object-Oriented Programming
- Object -Oriented Programming
- Programming paradigm
- Advantages
- Important Terminology
### What is OOPS ?
- A **Programming paradigm** that organizes software design around objects

**Programming Paradigm:** ia an approach used to solve problems with code.
- A style or "way" of programming.

### Differebt types of programming paradigms
- imperative   - when we start learning
- Functional
- Declarative
- Logical
- OOPS


OOP is based on **message** sent to objects.
- Objects **respond** to these messages by performing actions.
- Objects have their own **State** or set of **Attributes.


- **Class** is a blueprint which helps to create objects
- we can usee blueprints as many times we need to .
- Each object will have **State and Behaviour** . the set of actions that can perform.
- Objects can interact with other objects to perform complex functionalities.
- Programming paradigms are **not** mutually exclusive.
- The same program can have **multiple** programming paradigms.

### Advantages of OOPS
- Modularity
- Extensibility
- Reusability

## Classes : The Blueprints if Object Oriented Programming (OOP)
- Introdution to classes
- What they are used for 
- How to identify them
- Write a class header

### Classes
- A Blueprint for creating objects
- Class have state and behaviour
- Identify the Object + analye the state and behaviour of the objects +  Create a blueprint

### Naming conventions
- **Pascal Case** the first of each word should be capitalized, including the firstone.
- it is also known as **Upper Camel Case**

### Program description
- Problem Statement
- Nouns

### Class structor
- class have two main parts - header and body
- **Class Defination** - the implementation of a class in a programming language (Python)
- first line of a class definition of the class is called header
    - It specifies the name of the class and if it inherits from another class

```
class Backpack:
    pass
```
- **class Body** contains the elements of the "blueprint", including the attributes and behaviour of the objects.
    - Class attributes
    - __init__()
    - Methods


### Instances and Attributes
- **Instance** is an object created from class

### Self in OOPS
- classes define the state and the behaviour of the objects in a **generic** way.
- Its not specific. The code in the class has to work for **any** instance of the class.
- **self** is a generic way of refering to the current instance of the class.
- **seff** is skipped in the arguments list when we create an instance

### None  NoneType
- **None** is a special value that you can use to represent the absence of a value in your program. Its the only value of the **NoneType** data type.
- its commonly used to define a null variable or object.
- When a function doesn't explicitly retuen a value, it implicitly returns **None**.
- You can use **None** value in comparisons and expressions with the **is** and **is_not** operators.

### accessing the instance attribute

#### Dot Notation
- Syntax used to access the members of an object (its variables and methods).

### Default Arguments

- Defaults values assigned to parameters when their corresponding arguments are omitted.
- They must be the last parameters in the list of parameters.


### Modif the value of instance Attribute
- object.attribute = new_value
- self.attribute = new_value
