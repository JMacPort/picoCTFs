As usual we will grab the given files with `wget` which seems that one is a password cracker and the other is the flag which is encrypted. These must be stored in the same directory as per the instructions.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/9da31ac9-79e7-4d28-abd8-cbc43adcedae)

We will start by trying to read files using `cat` to understand what is going on. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/bba5ce2c-4f90-45ba-ab8e-96e427cfac13)

Clearly this is not the flag (yet) so now we will try the `level1.py` file, but before executing it we will read what it does with `cat`.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/761a7461-f643-4366-8a5e-d13025f7071d)

Reading into the second function we can see `if( user_pw == "691d"` which means the code following will be executing. There also seems to be a decryption method in there which is what we are looking for. Execute the `.py` script using
`python level1.py` and enter `691d` when it asks for a password. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/881ae8ce-1db9-4d9b-82ce-fb6883cddfe9)

And, once again, very simply we are able to grab the flag. 
