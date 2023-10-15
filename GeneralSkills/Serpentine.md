Again, download the given file and as usual `cat` into it to see how the script will work. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/b0b29d69-df06-42ef-bff9-e19a0fb8ba42)

We can see when the main function runs we will have three options, Print Encouragement, Print Flag, and to Quit. As we can see, the "Print Flag" option will not actually print the flag and says to check the
source code. My first instinct is to change the elif statement for "B" and make it so if the user enters "B" it will run the `print_flag()` function. 

Using vim, I will open the `serpentine.py` file and edit that `elif` statement as shown below. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/5945051d-256c-4b8d-a8c6-ce126c4db3c6)

And now this should print the flag when option "B" is selected. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/a94e415a-f2eb-4c3a-a5b7-f748e821651d)
