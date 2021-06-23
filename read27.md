# Django 

## Using Models
*Models are define the structure of stored data - including type, size, defaults, list options, text, etc*

- Django will communicate with the DB itself - you just pick the DB and models and django will handle the rest.

## Designing the Models

- When you know the models and fields, you need to know how the data relates.
- There are 3 types of relationships with django
  1.  `OneToOneField`
  2.  `ForeignKey` - one to many*
  3.  `ManytoManyField`
- multiplicities are the numbers on the UML diagram that show how many relationships to other models that model has.  

## Model Primer

- Defined in an apps models.py file
Fields:
  - can have any nuyber of fields
  - represents a coloumn 
  - rows (records) represent a columns value
  - field types are assigned with classes
  - contain type and validation criteria
  - also take in other arguments
  -   1. max_length
  -   2. help_text
  - name field is how to refer to it in queries and 
