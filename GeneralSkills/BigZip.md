Download the given `.zip` file and unzip it somewhere easy to access. As the title is "Big Zip" this most likely contains many files and directories. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/d3c84ac4-b34d-4b30-b35b-4ebbac8c1840)

Above is just some of the output. Now we know there are many different directories and files that we are dealing with so we will either be using some sort of `find` command or `grep` as these
both are able to sort through directories. As we don't know the specific file name here, `grep` is the more likely option as the flag is standard in all of these CTFs.

So, using the `grep -r pico` command will search the current directory along with all of its subdirectories until it finds a match to the search term, which here it is "pico".

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/d6ac2a6e-170e-4960-966b-8a7413117959)


