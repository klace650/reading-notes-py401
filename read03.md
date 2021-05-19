# Readubg abd Writing Files

## File Paths

*Three major parts*

1. Folder path - file location separated by slash (\ for windows)
2. File name - actual name of file
3. Extensions - suffix/file type (.md, .gif etc)  

## Line endings

*It is important to show when the line stops and begins new line - think about morse code of telegrams*

``\r\n`` is the standard for carriage return and line feed

**NOTE** - Unix will start ``\n`` on a new line

## Character Encoding

*Important to note that ASCII and UNICODE will encode character differently - but also 128 time not*

## Opening and Closing a File

ok => ``file = open("file name")``  
best => ``with open("file name", 'r') as reader:``

*Its important to close the file when you're done to reduce unwanted behavior*

`r` : open for reading  
`w` : open for writing  
`rb` or `wb` : open in binary  

## How to read files:

`.read(size=-1)` : will read whole file with -1 as the size  

`readline(size=-1)` : reads entire line with -1 or nothing passed in 

`.readline()` : returns lines as a list 

## Example of how to iterate though file:

*copied from https://realpython.com/read-write-files-python/#file-paths*

``with open('dog_breeds.txt', 'r') as reader:  
  for line in reader:  
    print(line, end='')``

