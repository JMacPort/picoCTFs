We will grab the given file and check out the `cat` output of the file.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/82dd611d-4929-4713-9b88-eef3f984cd3d)

Since this challenge is tagged with base64 and the output looks base64 we can pressume that this will need to be decoded. Going to an online converter shows that this will need to be converted multiple times
as it returned another base64 string which will be annoying if it continues. We can use Python to automate this process with a pretty simple function.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/095806f3-1d0d-4135-9b75-6d80d34c22cd)

Creating a new file called `script.py` and then using vim to edit this file we can open the `enc_flag` file, store it into a variable and then convert that variable from base64 to utf8 which makes it readable. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/663b1239-bac4-42a5-b98f-c17ad6abe29e)

This will run through the decoding process to eventually print the flag. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/ed9e2c7f-4a25-4852-9378-482cbb1b24da)
