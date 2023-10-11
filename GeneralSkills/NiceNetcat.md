It gives us a command to run ```nc mercury.picoctf.net 43239```. This is invoking the netcat tool and checking over port 43239 for any reponses.

We can see the output is a list of random numbers. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/56d7ecfe-b95d-4f8c-9741-3ab2a710b0ad)

To make sense of these numbers I used a simple Python script utilizing the ```chr``` method to convert an integer to a unicode character. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/16357904-a6ac-4717-bb8f-3a2dd8e4b87b)

You can see above that each of the numbers was added to a variable named ```chars``` and then an empty ```flag``` variable was created. 
This utilizes a for loop to get each item in the array and convert them to a character, which is then shown in the output when the script is run.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/10d158e8-1371-45ce-9e00-485e8d0b5093)
