# Classes and Objects

"Objects are an encapsulation of variables and functions into a single 
entity"

## Basic Example
```class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

```

*Note the `self` parameter for later

You can access the variable by creating an object and making an instance of that class - then using (i guess) dot notation to access the variable.

`access = MyClass()` <-- creates instance of myclass set to a variable now.  
`access.variable` <-- and this goes in and grabs that variable  
`access.function()` <-- this works the same way but makes an instance of the function inside the object.

---

# Thinking Recursivley 

Ok dang this santa analogy helps explain recursion very well. 

This summarizes recursion well to I think:  

`This (recursion) means that the function will continue to call itself and repeat its behavior until some condition is met to return a result.`

Basically, divide up the problems as many times as possible to make the sub-problems so trivial and small that they don't need further division. 

# Python Fixtures and Coverage

## Fixtures:

*These are groupings of tests that are available to all tests across your code*

Fixtures are defined using th ``pytest.fixture`` decorator, along with function def.

this is how it'll look in pytest
```
@pytest.fixture
def simple_file():
   return StringIO('\n'.join(['abc', 'def', 'ghi', 'jkl']))
```