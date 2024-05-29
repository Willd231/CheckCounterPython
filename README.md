# CheckCounterPython
Check Counter program in Python

I made this during my first year as a computer science undergrad while working as an OPS student under Anish Damodaran, a researcher at the Florida Space Institute. 
The main purpose of this program is to check the relationship between the data coming from the FPGA and another program aiming to process it. The way it works is that it takes in a filename, and by using the glob module, it returns all files within the same directory with a similar filename as dictated by the wildcard. After that, a triple nested for loop is implemented: 1st layer is to iterate through each file returned by the glob function, 2nd layer iterates through the current file in chunks of 8448 bytes, and 3rd layer compares a copy of the first 8 bytes to the first 8 bytes of every chunk and returns any spot where they don't match up.

