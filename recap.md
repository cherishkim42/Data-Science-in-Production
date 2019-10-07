# Data Science in Production
​
​
## What is Flask?
Flask is a micro framework in python that allows us to make API's.
​
### - What are two advantages of `flask_restplus` over just flask?
1. Automatically generated UI interface
2. Automatically generated documentation
3. Builtin ArgParser
​
## What are the steps to deploy ML/DL model to cloud?
1. Create model -> Train Model -> Save Model
2. Make an api interface to interact with the model
3. Dockerize the api
4. Deploy
​
### - Two ways to deploy on AWS?
1. Amazon ECS (Elastic Container Service)
2. Beanstalk -- This way doesn't requiring Docker
​
## Bigger Data
​
### - Data cannot fit in memory with limited resources, what options do we have?
1. Use a generator
​
### - Two frameworks for big data
1. Pyspark
2. H2O
​
## Advanced Programming
​
### - What is a decorator?
A function that wraps a function to extend the functionality of the wrapped or inner function
```python
def print_hello_first(func):
    print("Hello")
    return func
​
@print_hello_first
def do_stuff():
    print("Doing the stuff")
​
---------------------------------------
> do_stuff()
"Hello"
"Doing the stuff"
```
​
### - Class methods, abstract methods, class variables, instance variables, ABC class ...
​
## Functional Programming: map, filter, reduce, lambda ...
### Why do we need map/reduce?
It is not required although using the builtin map function instead of (for example) a list comprehension allows python to more efficiently distribute the computing power among your computers CPU cores.
​
### Normal syntax vs Pyspark syntax
​
|             Normal             |             Pyspark           |
|:-------------------------------|:------------------------------|  
|   `map(function, collection)`  |   `collection.map(function)`  |
| `reduce(function, collection)` | `collection.reduce(function)` |
​