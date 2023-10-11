We will be grabbing the file again using `wget` and it specifically states to not run the file. Using context clues, we can assume that the ```strings``` command will be used to get any relevant strings from the given file. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/5b2d9adb-fd5a-4bc2-8127-4a0a8db85886)

The output is clearly a bunch of separated strings but to find the flag we will use `grep`. This will allow us to filter the output to find the flag much easier than searching through each string.

`strings strings | grep picoCTF` finds the flag perfectly with no excess information. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/1fe33b3e-c86a-4ab0-ac14-fc1a2b5e6126)




