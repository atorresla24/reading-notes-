# Reading class 03

## Read & Write Files in Python

- Reading and writing files is one of the most common tasks in Python
- A **file** is a contiguous set of bytes used to store data
- Files are composed of three main parts:
  - **Header** is metadata about the contents of the file (file name, size, type, etc)
  - **Data** is the contents of the file 
  - **End of file (EOF) is a special character that indicates the end of the file
- To access a file a **file path** is required and it is broken up in three major parts:
  - **Folder path** is the file folder location on the file system where subsequent folders are separated by forward slash
  - **File name** is the name of the file
  - **Extension** is the end of the file path pre-pended with a period used to indicate the file type
- An encoding is a translation from byte data to human readable characters
- Two most common encodings are:
  - **ASCII** which can sore 128 characters
  - **Unicode** which can contain 1,114,112 characters
- To open a file 'var_name = open(file_name)'
- To close 'reader.close()'
- Characters to go through files:
  - 'r' = open for reading
  - 'w' = open for writing
  - 'rb' or 'wb' = open in binary mode
- Three different categories of file objects:
  - **Text files** is the most common file that you'll encounter
  - **Buffered binary files** is used for reading and writing binary files
  - **Raw binary files** is generally used as a low level building block for binary and text streams
- Methods:
  - .write(string)
  - .writelines(seq)

## Exceptions in Python

- Use *raise* to throw an exception if a condition occurs
- If condition is *true* the code will continue if it is *false* then the program will output an *AssertionError*
- A *try* and *except* block in Python is used to catch and handle exceptions
  - A *try* will run a piece of code and an except will run another piece of code if there is an exception
  - An *else* will run another piece of code if there is no exceptions
- By using *finally* any code after this will always run 

## Things I want to know more about

- I want to know more about how accessing files and overwriting them will help me in future coding
- I want to know how I can use try and except blocks to be able to catch errors in my code and how they can help me fix my code

