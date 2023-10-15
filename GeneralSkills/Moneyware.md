This CTF has nothing to download and simply asks for an answer to the following passage. 
![image](https://github.com/JMacPort/picoCTFs/assets/145376972/c927b90e-7f24-47fb-81ed-4ab4eb0f8cda)

After trying many different variations of "Ransomware" I realized that the Bitcoin address must be of some use and dug around on [chainabuse](https://www.chainabuse.com/address/1Mz7153HMuxXTuR2R1t78mGSdzaAtNbBWX). I found a report as below. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/edd2cc0b-f3b8-4d65-ae0a-039658a8e54b)

This takes us to a report of a Ransomware malware named "Petya" which I then tried as the flag. 

Using the correct format `picoCTF{Petya}` was the correct flag and simply relied on simple blockchain knowledge. 
