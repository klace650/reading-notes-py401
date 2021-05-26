# List Comprehensions
https://www.pythonforbeginners.com/basics/list-comprehensions-in-python

*Concise way to create a lists*

- uses brackets around an expression followed by a for clause - then zero or more if clauses.
- expressions can be anything
- always returns a list

The old way/how I would have done it?
``` 
new_list = []
for i in old_list:
    if filter(i):
        new_list.append(expressions(i))
```
Now do this
```
new_list = [expression(i) for i in old_list if filter(i)]
```
``new_list`` - the new list (result)
`expression(i)` - based on the var use for each element in the old list
`for i in old_list` - the word for followed by "new" var followed by the old_list words
`if filter(i)` - apply a filter with if statement
`new_range = [i * i for i in range(5) if i % 2 == 0]` == `*result* = [*transform* *iteration* *filter* ]`