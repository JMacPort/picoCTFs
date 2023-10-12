Just like PWCrack1 we will `wget` the given files and store them in the same directory to ensure compatibility. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/9b0a825b-b366-4a35-acde-58fadba565ab)

Once again, we will use `cat` on both of the files and the output will be shown below. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/a37f728c-864f-4d79-8d0e-574391e587ff)
![image](https://github.com/JMacPort/picoCTFs/assets/145376972/09bafd28-4717-44a3-bd1d-c638e52a30bc)

The flag text files again gives no help to decode the flag, but in the `.py` file we can see it has some hex characters which we can use another python script to decode quickly. In another terminal open `python`.
Copy over the given hex characters into a variable and then print the variable to get the password needed. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/3cdf10aa-1441-4547-8d5c-21e426b3e103)

Back over in the original terminal we can run the script with `python level2.py` and input the password from the other terminal.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/31577674-edd0-452e-9b2a-ec5c3bffe673)
