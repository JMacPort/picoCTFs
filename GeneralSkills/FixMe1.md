Lets grab the file as needed using `wget` noting that we will be fixing an error within this script. To do so, lets run the script first to see if it produces an error with `python fixme1.py`. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/5815b5f5-f7c9-4bf4-b20d-48e02b8345ed)

To edit this, we can use the vim tool that allows us to edit files using `vim fixme1.py`. This should open the `.py` file in the text editor. Using vim can be daunting but for simplicity, pressing `i` will allow you insert, or delete in our case.

Using the arrow keys navigate down to the "p" in the `print` statement and press delete to remove the indentation. Now press escape to stop editing. To save the file use `:w` to write it to the file and then `:qa` to exit vim.

Now run `python fixme1.py` and the error should be fixed. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/b4c64abd-53b0-46d8-a214-d271995f1e3e)
