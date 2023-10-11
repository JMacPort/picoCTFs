Per usual we will be grabbing the files using the ```wget``` command. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/9fecec90-30f6-4e94-8f54-79d4067ebc5e)

Now that we have all three files, it is best to call ```cat``` on each to see if we can read the contents to figure out what we have to work with. 

In ```ende.py``` we can see the following variable ```help_msg```.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/3ceab2fa-9622-4fc8-847d-9a55bdd308cb)

This is telling us that we need to decrypt a file named ```pole.txt``` which does not currently exist. Further down in the ```ende.py``` file we can see a function that takes a password and then will decrypt a given file
when given the ```-d``` flag. So, we will copy the contents of the encrypted ```flag.txt.en``` file into a new file called ```pole.txt``` and will assume the password it is asking for is located in the ```pw.txt``` file.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/459147a7-b8c7-4c6f-b481-05ee84b4afdb)

Now, we can called the ```ende.py``` script using the format given in the variable above using the following ```python ende.py -d pole.txt```.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/87d7c16f-75c6-4ed5-ad39-7a2fe9d44c0c)
