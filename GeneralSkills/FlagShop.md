We see this is another netcat challenge but it also seems to include the source code of the page we are grabbing in a file titled "Source". Upon reading into "store.c" with `cat` we get the code for a program.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/66797702-2317-437e-afc7-f211e2c5f9f9)

In this it says "fake flags" are 900 dollars and the presumably real flag is 10,000. The hint for this task regard the two's compliment which means the highest number that can be represented is `2,147,483,647`. So, adding 1 to this number effectively
switch it to be a negative `-2,147,483,648`. Now since we know each real flag is 10,000 we have to figure out how many flags we would need to change the total payment to a negative. But, before we continue here I noticed that there is only one real flag in stock. 
This means that any number over one will just get passed over. So now we have to find how many fake flags instead we can buy to get the balance due to a negative. This brings the total number of fake flags to 2,386,093. 
Rounding this up a bit to ensure our numbers are correct we can use 2,400,000 as the number of fake flags we will attempt to buy. 

So connecting to netcat we can try our solution and we can see that this worked perfectly. This flipped the final cost to be a negative, which in turn increased our available balance. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/e014a9c5-b3bf-4d4b-ada7-14d34065b32e)

Now we should be able to go ahead and purchase a real flag which again worked perfectly to complete the challenge. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/97f2a900-04da-4b92-a43e-65e823b623f9)
