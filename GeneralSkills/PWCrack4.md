Once again this has us grabbing 3 different files but contains 100 possible passwords so brute forcing will be a last resort option.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/99612826-957a-4852-9d2f-df49d8c0bf05)

Again below will be the output of trying to read each file in case there is some sort of hidden piece of text within them. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/b8acd7e6-4c23-4c21-bdec-09ff446ec054)
![image](https://github.com/JMacPort/picoCTFs/assets/145376972/deee494f-e92b-4460-a130-282cfbfe4e5f)
![image](https://github.com/JMacPort/picoCTFs/assets/145376972/9291fd02-919c-46dc-b7bf-98fc4d5378b6)

As the first two files do not really provide any sort of assistance, we will look at the script and note the amount of possible passwords. Since these are given, we can use python to iterate over each password and try it in the function. 

Stealing some code from the original script, we need the hashing function that encodes the password `hash_pw`, the list of possible passwords in the `pos_pw_list` array and then the `correct_pw_hash` variable.

Using those variables along with a custom `for` loop to iterate each password we come up with a script like below.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/fb2b5428-fe70-4fdb-bc4a-34e00b2c5096)

Be sure this script is stored in the same directory as the rest of the files and then we can run it using `python script.py` to get the password. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/16e47d64-0b96-4369-a125-3b8d05087a9b)

Then we can now use this password when we run the `level4.py` script to get the flag.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/356d5b98-28e7-4f68-811b-423eba406307)
