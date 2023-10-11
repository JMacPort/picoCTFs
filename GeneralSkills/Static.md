Once again we grab the given files with ```wget```. This gives a bash script named ```ltdis.sh``` and file named ```static```. Using ```cat``` on the ```static``` file doesn't provide any meaningful output,
but using it on ```ltdis.sh``` allows us to read what the bash script will be accomplishing. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/18502811-4296-43c9-9cb4-121ca51159d9)

After attempting to simply run the bash script using ```bash ltdis.sh``` we can see "Disassembly failed!" but the output gives more meaningful advice as well. It looks as though a file were supposed to be passed in to disassemble. 
Now we can try passing in the ```static``` file into the script using ```bash ltdis.sh static```. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/0e31b3ec-94a6-4386-b164-2384c542d998)

We are given the above output and now we need to access ```static.ltdis.strings.txt``` to see if we can access the flag or if there will be more steps.
This gives a bunch of different lines of random strings and more. But if we actually open the text file in Mousepad, we can ```ctrl+f``` to search the file and find if there is anything containing the flag.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/f5aa190c-d6ff-4539-bcf0-86965d7c6e1a)

Which we can see worked and have found the flag for this section.

