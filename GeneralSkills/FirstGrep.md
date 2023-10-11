The first step as usual will be grabbing the file using `wget` and then we will try to `cat` into the file. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/2b592a3c-def8-41ec-9d67-2ac5345c070a)

This hits us with a wall of characters but no easy way to actually find the flag we are looking for. This is where `grep` will come in handy. If we do `cat file | grep picoCTF` this will allow
us to quickly search the file to find the flag. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/46f2349d-90a6-4d21-9744-85ff6616288a)

And very easily, we are able to grab the flag. 
