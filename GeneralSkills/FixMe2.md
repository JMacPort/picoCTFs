Once again download the given `.py` file with the `wget` command. Running this file using `python fixme2.py` shows that the equals sign operator is being used incorrectly, so we will need to edit this in vim again.
In vim, press "i" to go into insert mode and arrow down to the final if statement and add another equals sign next to the one that is already there. This now says, if the flag is equal to an empty string it will print an error, 
otherwise it will print the flag. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/38ae4165-00c0-4f6a-9c0c-ee4f43a88ef5)

Once editedm press escape and then `:w` to write the changes and then `:qa` to exit vim. Run the file once again with `python fixme2.py` to get the flag. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/d055c627-b267-4b92-8273-fc33d9c2f5cd)
