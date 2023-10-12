As laid out in the description the first thing we should do is see the response given from the port `nc staturn.picoctf.net 52682`.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/61ebb0a4-8649-4fee-b451-82462935bc8a)

It gives us the output of the beginning of the flag and then some hex characters that we can put into python to get the rest. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/798833ce-f709-4568-a47e-1f75418d71b2)

Simply adding the given response to a varible, python knows that `chr` is meant to convert hex characters and comining the elements gives the flag as shown above. 
