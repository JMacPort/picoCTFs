We will download the given file as usual using `wget` to our directory. This gives us a text file called "lyrics.txt". 

Using `cat` seems to gives us lyrics to a song.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/d141c2be-4c7d-4853-8850-bc40c5f79a7b)

Since I am completely lost at this point I checked the hint and it asked "Do you think you can master rockstar?". Which I then discovered was a programming language and found an online intepreter for. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/2de710b7-919b-4492-8a23-fca2381d9b55)

Now seeing the output, we know this is ASCII characters which can then be converted once again. And now inputting this into picoCTF following the correct format `picoCTF{rrrocknrn0113r}` completes this challenge. 
