This is another suimulation to connect via SSH. If we `ls -la` we see a few files here, notably the `useless` and `.profile` files.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/ebc371a9-e589-4d9f-9ea1-a7740c856fc0)

Calling the program `./useless` directs us to read the code first, which then we can see with `cat`. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/38eea05e-4a19-4796-ad3a-afbd340f59d1)

We can see the very bottom `else` statement directs us to "Read the manual" which can be done using `man useless`. In doing this, the flag appears in the bottom under authors and also shows the syntax to run the program. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/0e62db2f-bdf0-4697-b881-9b59cd978773)
