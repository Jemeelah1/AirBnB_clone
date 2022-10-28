# AirBnB_Clone

![](https://camo.githubusercontent.com/a8cd2eef2325c425519095dc2501111e630a77eddb454938c527cb82ea9c3aeb/68747470733a2f2f73332e616d617a6f6e6177732e636f6d2f696e7472616e65742d70726f6a656374732d66696c65732f686f6c626572746f6e7363686f6f6c2d6869676865722d6c6576656c5f70726f6772616d6d696e672b2f3236332f4842544e2d68626e622d46696e616c2e706e67)

# Description :label:

## 

HBNB is a complete web application, integrating database storage, HTML/CSS templating, API, front-end and others.

This team project is part of the ALX School Software Engineering program. </br>
It represents the first step towards building a full web application: the AirBnB clone.

This first step consists of:
- a custom command-line interface for data management,
- and the base classes for the storage of this data.

## Usage í²»

The console works both in interactive mode and non-interactive mode, much like a Unix shell.
It prints a prompt **(hbnb)** and waits for the user for input.

Command | Example
------- | -------
Run the console | ```./console.py```
Quit the console | ```(hbnb) quit```
Display the help for a command | ```(hbnb) help <command>```
Create an object (prints its id)| ```(hbnb) create <class>```
Show an object | ```(hbnb) show <class> <id>``` or ```(hbnb) <class>.show(<id>)```
Destroy an object | ```(hbnb) destroy <class> <id>``` or ```(hbnb) <class>.destroy(<id>)```
Show all objects, or all instances of a class | ```(hbnb) all``` or ```(hbnb) all <class>```
Update an attribute of an object | ```(hbnb) update <class> <id> <attribute name> "<attribute value>"``` or ```(hbnb) <class>.update(<id>, <attribute name>, "<attribute value>")```

### Interactive mode (example)

```bash
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb)
(hbnb)
(hbnb) quit
$
```

### Non-interactive mode (example)

```bash
$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
```

## Testing :straight_ruler:

Unittests for the HolbertonBnB project are defined in the [tests](./tests)
folder. To run the entire test suite simultaneously, execute the following command:

```
$ python3 unittest -m discover tests
```

Alternatively, you can specify a single test file to run at a time:

```
$ python3 unittest -m tests/test_console.py
```
## Purpose of Project

The purpose of this project is to understand how to:

- create a Python package
- create a command interpreter using the `cmd module`
- serialize and deserialize a Class
- write and read a `JSON` file
- manage datetime
- use `*args` and `**kwargs`
- handle named arguments in a function

## Requirements

### PYTHON SCRIPT REQUIREMENTS

- allowed editors: `vi`, `vim`, `emacs`
- the first line of all files should be exactly `#!/usr/bin/python3`
- all code should use the `PEP8` style (version 1.7.*)
- all files must be executable
- all files will be interpreted/compiled on `Ubuntu 14.04 LTS` using python3 (version 3.4.3)

### PYTHON TEST CASE REQUIREMENTS
- all test files should be in the folder tests
- all test files should be text files (extension: .txt)
- all test files should be executed using the command `python3 -m doctest ./tests/*`
- all modules should have documentation `python3 -c 'print(__import__("my_module").__doc__)'`
- all functions (inside and outside of classes) should have documentation python3 -c 'print(__import__("my_module").my_funct\ ion.__doc__)'
