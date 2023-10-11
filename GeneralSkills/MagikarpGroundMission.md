Here we are given an ssh session that we need to access and are given a command to enter the session. Upon entering the command and the correct password we are now communicating via ssh.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/b569e301-b799-4869-928f-6d4c820ae67c)

Using ```ls``` we can immediately see two files that show the flag should be broken up into three parts. So, first we will ```cat 1of3.flag.txt``` to get the first part of the flag. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/f0f71323-1762-4665-853e-d79bfba40c70)

Now we will ```cat intructions-to-2of3.txt``` to find the next set of instructions. Which tells us that we will need to access the root directory. We can do this by ```cd ../../../..```. This will bring us backwards 4 directories. 
And now ``ls`` again to see ```2of3.flag.txt```. Using `cat` to read this text file we will get the second part of the flag. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/41f94a9b-b133-465e-bb3d-b94923c99d83)

And finally, `cat intructions-to-3of3.txt` to find how to access the final part of the flag. This tells us that we need to go to the home folder using `cd ~ `. Here we will see the `3of3.flag.txt` and the final piece of the puzzle. `cat` into this file and
this CTF has been completed. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/a1aaff42-bceb-4a44-9430-eab4ef5d316b)

