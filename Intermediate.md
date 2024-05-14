# INTERMEDIATE - QUESTIONS
## I/O

## Task 1

Write a script that searches for all files with a `.txt` extension in the current directory and writes their names to a file named `txt_files.txt`.


## Task 2

Write a program that creates a directory named `test_directory`, then creates a file named `sample.txt` inside that directory. Use time library to provide 10 seconds delay time (time.sleep(10)) and finally delete the directory along with the file.

Give a print message when both the directory and file created and deleted.

## Task 3

Create a script that reads a text file named `easy-task1.txt` and count the number of words it contains.
In the same script copy the same file content to a new file named `easy-task1-copy.txt` and change its permissions to be read-only.

## Task 4
Write a script that uses the io module to read a file named `easy-task5-copy.txt` (from Task 3) line by line using `readline()`, checks if the stream is `readable`, `writable`, and `seekable`, and writes each line to `intermediate-task4.txt` in reverse order.

#### Hint: use file.readable(), file.writeable(), file.seekable()



## Task 5
Create a script that searches for `the` string in all `.txt` files within current  directory `.` and its subdirectories, replaces it with `DCI` string, and saves the changes. Also, log the changes to a file named `changedlog.txt`.


## Libraries 

### Task 6
Write a script that takes command-line arguments for a `filename` and a `word`. The script should read the file and count how many times the word appears in that file.

#### Hint: script execution should be like : `python script.py <filename> <word>`


### Task7

Create your own custom package that calculates the total size(in bytes) of all files in the current directory. Build and publish this on Pypi, you should be able to import your package and execute the module. 

The logic required is :

### Calculating the total size of all files in the current directory

```
import os
def total_directory_size():
    total_size = sum(os.path.getsize(f) for f in os.listdir('.') if os.path.isfile(f))
    return total_size
print(f'The total size of all files in the current directory is {total_directory_size()} bytes.')

```
