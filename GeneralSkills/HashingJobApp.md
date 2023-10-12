Again we will use the given `netcat` command `nc saturn.picoctf.net 53683` to investigate the output. 

We can see it is asking for an md5 hash of the phrase "cleaning the bathroom" which we can do in python once again. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/e9078e8a-8c3a-4207-9809-8f5fb817ec62)

The task requires this done three times in somewhat quick succession, or it may close the connection. Show below is the python code for all 3 attempts.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/cbacc367-527e-48a8-ab30-930232abeed8)

Here, we imported the `hashlib` library to gain access to hashing algorithms and then created a variable that will store the hashed phrase using the md5 algorithm. 

Then we print out the `hexdigest()` of the encoded variable which gave us access to the flag. 
