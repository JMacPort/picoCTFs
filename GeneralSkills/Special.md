This challenge appears to be some sort of ssh connection but no other details are really given within the description. Connecting to the shell immediatly presents confusion. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/4850ffdf-4fcf-40df-9f50-3db0bc0df96c)

Reading back into the description of the challenge we can see that every word is supposed to be properly spelled and capitalized behind the scenes. So, we are dealing with some sort of program that has to be reverse engineered. 
This one had me completely stumped and I eventually had to find the proper way to complete it. Using [Josephs](https://josephkimiri.github.io/posts/Special/) write up I discovered there are different ways to enter input into a shell. 

Through their assitance we can note that using `${parameter=ls}` gives us an alternative way to enter commands into a shell. 
![image](https://github.com/JMacPort/picoCTFs/assets/145376972/8d6026be-bed0-49c3-a61f-41c7fe7c7af8)

We can now see inside of the directory "blargh" there is a `flag.txt` file which can be read using `${parameter=cat < blargh/flag.txt}`.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/654fab9d-ea58-47e0-bcfb-d5d4dfc41efb)
