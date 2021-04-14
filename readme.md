# Clean Code

#### Table of Contents
- [Clean Code](#clean-code)
      - [Table of Contents](#table-of-contents)
  - [What is "clean code"?](#what-is-clean-code)
  - [Naming](#naming)
    - [Why Good Names?](#why-good-names)
    - [Variables & Constants](#variables--constants)
    - [Functions/Methods](#functionsmethods)
    - [Classes](#classes)
  - [Name Casing](#name-casing)
    - [snake_case](#snake_case)
    - [cameCase](#camecase)
    - [PascalCase](#pascalcase)
    - [kebap-case](#kebap-case)
  - [Naming Variables, Constants & Properties](#naming-variables-constants--properties)

## What is "clean code"?

- if your code takes some time to understand, it may be a sign that it's a bad code.
- not about whether code works or not.
- your code is readable and understandable
- reduce cognitive load
- concise and to the point.
- avoid intuitive names, complex nesting and big code blocks

## Naming

### Why Good Names?

- names should be meaningful
- define what it is or what it does

```js
const us = new MainEntity();
us.process();

if (login) {
  //...
}
```

The above code is very hard to understand what `us` is and so on. We can fix the above code as follow:

```js
const user = new User();
user.save();

if (isLoggedIn) {
  //...
}
```

**Naming well can allow readers of your code to understand without going through much detail.**

```js
const user = new User();
```

```js
database.insert(user);
```

```js
if (loggedIn) {
  /*...*/
}
```

### Variables & Constants

- Data containers
  - user input data
  - validation results
  - a list of products
- nouns
- short phrases with adjectives

```js
const userData = {
  /*...*/
};

const isValid = false;
```

### Functions/Methods

- commands or calculated values
  - send data to server
  - check if user is valid
- use **verbs** or short phrases with **adjectives**

```js
sendData();

inputIsValid();
```

### Classes
- use classes to create objects
  - user
  - product
  - http request body
- use __noun__ or __short phrases__ with __nouns__

```js
class User { /*..*/ }

class RequestBody { /*..*/ }
```

## Name Casing

### snake_case
- examples:
  - is_valid
  - send_response
- used languages:
  - python
- used for:
  - variables
  - functions
  - methods
### cameCase
- examples:
  - isValid
  - sendResponse
- Languags:
  - Java
  - Javascript
- For:
  - variables
  - functions
  - methods

### PascalCase
- examples:
  - AdminRole
  - UserRepository
- Languags:
  - Python
  - Java
  - Javascript
- For:
  - Classes
### kebap-case
- examples:
  - \<side-drawer\>
- Lannguages:
  - HTML
- For:
  - Custom HTML elements

## Naming Variables, Constants & Properties
- Value is an __Object__?
  - Describe the value
    - user
    - database
  - Provide more details without introducing redundancy
    - authenticatedUser
    - sqlDatabase
- Value is __Number__ or __String__?
  - Describe value
    - name
    - age
  - Provide more details without introducing redundancy
    - firstName
    - age
- Value is __Boolean__?
  - Answer a true/false question
    - isActive
    - loggedIn
  - Provide more details without introducing redundancy
    - isActiveUser
    - loggedIn