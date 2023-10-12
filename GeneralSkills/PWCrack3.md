Again download the files to the same directory, but this time an additional file is included to give us three. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/4740100e-b44a-40d2-88e0-275a11c5558b)

We will `cat` through each file to examine the output for anything that may be able to help, where each output will be below.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/79847fa8-a16d-464a-b187-aabbcde4981c)
![image](https://github.com/JMacPort/picoCTFs/assets/145376972/d763e1d3-efd5-49e0-b724-1f2b7c3d65a5)
![image](https://github.com/JMacPort/picoCTFs/assets/145376972/4373d3ae-c796-41eb-b3e2-f5649cbb2bc3)

**I only included the lower half of the python script as the top funtion is noted to not be able to help find the flag**

Using a binary visual editor such as bvi, as noted in hint 1, we can view the contents of the `.bin` file. Which after examining contains some hex values in which we can check in a converter. 
The binary reads: Null, Escape, "á", Unit Separator, "o", "\", Device Control 1, "`", "[", Enquiry, ">", File Separator, "ê", "(", "à", "."

This gives virtually no assistance, so moving onto the `.py` script we can see at the bottom there is a list of seven passwords that are possibly the password. So, we can brute force the password using
one of these given passwords. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/3bdd9db0-8d06-4eab-8e36-346110143687)
