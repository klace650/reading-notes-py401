# Global and Local Scope


## Global Scope
In order to access a variable stored outside of a function - you need to put a scope statement into the function.

```
# correct example
counter = 0  # A global name
def update_counter():
    global counter  # Declare counter as global
    counter = counter + 1  # Successfully update the counter

update_counter()
counter

update_counter()
counter

update_counter()
counter
```

*Typically considered bad form to use these feature - its best to look at your code and see if there is a better way to do it*

- The 'lazy' way to do it is to just wrap the global statement inside the function
- But this can be hard to debug

## Nonlocal Statement

- Can be accessed from inner functions, but can't be modified.
- To modify, need to use `non-local statment`
- Using this will access var names inside a nested function
- Can't be used outside of a nested function
- Cannot create lazy statements

```
def func():
    var = 100  # A nonlocal variable
    def nested():
        nonlocal var  # Declare var as nonlocal
        var += 100

    nested()
    print(var)

func()
```

# Big O Vidya

- Big O is really all about how well an algorithm can handle more data.
- All about scale and big O measures that increasing amount of data.
- Big O is a way to compare
- Gives you worst case scenario

## Different Types of Complexity:

- Constant
- Log
- Linear
- Log Linear
- Polynomial

