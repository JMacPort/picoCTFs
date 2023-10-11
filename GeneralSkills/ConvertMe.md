Getting the file iusing `wget`, we can then `cat` to read more about what the script will be doing. We can see again the `flag_enc` contains a bunch of hexadecimal characters and then a variable named `num` which contains a random
number between 10 and 101. A print statement is used to ask the user what the number will be in binary. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/ac8522c7-b991-4787-a09a-d455aec879ff)

Lets run the script and get the correct conversion by using `python convertme.py`. And then it is as simple as converting the given number to binary.

Binary is very simple, it consists of 8 digits with the digits starting at the left to right representing: 128 64 32 16 8 4 2 1

To get the conversion you must figure out which of the numbers are used in the calculation. For ours, we got 67. So, you start at the highest possible number that can be used and work backwards. 
Here we can start at 64 and then add the 2 and the 1. Which will look like `01000011`. Each `1` represents that numbered "turned on" in a way. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/68904068-4c30-4e2f-b31a-795a71284638)
