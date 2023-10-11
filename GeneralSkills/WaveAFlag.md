We will grab the given file using ```wget``` as usual.

Technically calling ```cat``` on the file given will get the CTF flag but it is not the best way to get this flag. 

To do so, we will change the permissions of the file to an executable by doing ```chmod +x warm``` and then can run the file with ```./warm```.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/f99375e4-2d9a-416c-b5fd-f8a8b5e6905e)

We can see that it is telling us to run the file again but this time use a ```-h``` flag.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/d4e9866b-19b2-4d39-903c-07e30da5eede)

This will produce the above flag.
