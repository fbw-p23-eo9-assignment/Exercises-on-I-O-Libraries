# EASY - QUESTIONS

## I/O: 


### Task 1

Write a Python script that reads the contents of a text file named `easy-task1.txt`, converts all text to uppercase, and writes the result to a new file named `task1-output.txt`.


### Task 2

Create a script that appends the current date and time to a file named `log.txt` each time it is run.


### Task 3

Create a script that lists all files and directories in the `/home` directory  and in the `.` currect directory separately and writes each list to a files named `home_directory_list.txt` and `currect_directory_list.txt`.
#### Hint:  home= os.path.expanduser('~')


### Task 4

Write a script that merges the contents of two files, `easy-task1.txt` and `easy-task5.txt`, and writes the merged content to a new file named `merged-easy-task4.txt`.
The script should also print the size (in bytes) of the same file `merged-easy-task4.txt`.


### Task 5

Create a script that renames a file named `easy-task5.txt` to `new_easy-task5.txt`. The script should prompt the user to enter a string and then write that string in a new line to the same file `new_easy-task5.txt`.


### Task 6

Create a script that reads a text file named `easy-task5.txt`, converts its content to bytes using UTF-8 encoding, then converts those bytes back to a string, and writes both the byte representation and the reconverted string to another file named `output.txt`.



## Libraries 

### Task 7
Create a script that takes a filename and a string as arguments and writes the string to the file. Use the argparse module for argument parsing.

### Task 8

Temperature Conversion Package:

Your task is to create a Python package called temperature_conversion that should consist of at least 4 modules. Each module should be responsible for one distinct temperature conversion (Celsius to Fahrenheit, Fahrenheit to Celsius, Celsius to Kelvin, Kelvin to Celsius). In your modules, you can use basic arithmetic operations.

Outside the package, write a Python script that uses the aforementioned modules to perform some temperature conversions test.

Hint: Remember about the __init__.py file inside the package folder!

Create the package structure:
``` 
temperature_conversion/
    __init__.py
    celsius_to_fahrenheit.py
    fahrenheit_to_celsius.py
    celsius_to_kelvin.py
    kelvin_to_celsius.py
test.py 
```

`test.py` will have the following code:
```
from temperature_conversion.celsius_to_fahrenheit import celsius_to_fahrenheit
from temperature_conversion.fahrenheit_to_celsius import fahrenheit_to_celsius
from temperature_conversion.celsius_to_kelvin import celsius_to_kelvin
from temperature_conversion.kelvin_to_celsius import kelvin_to_celsius

temp_c = 25
temp_f = 77
temp_k = 298

print(f"{temp_c}°C to Fahrenheit: {celsius_to_fahrenheit(temp_c)}°F")
print(f"{temp_f}°F to Celsius: {fahrenheit_to_celsius(temp_f)}°C")
print(f"{temp_c}°C to Kelvin: {celsius_to_kelvin(temp_c)}K")
print(f"{temp_k}K to Celsius: {kelvin_to_celsius(temp_k)}°C")
```

### Task 9

Write a script that performs a basic arithmetic operation (add, subtract, multiply, divide) based on command-line arguments. The script should take three arguments: two numbers and an operator.

#### Hint: script execution should be like : `python script.py <num1> <num2> <operator>`