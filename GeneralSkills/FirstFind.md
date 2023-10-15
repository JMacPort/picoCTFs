The given file this time is compressed so once downloaded, we will need to run `unzip` to get the contents and for simplicity sake we can then run `rm files.zip` to have only the uncompressed directory. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/103eb34b-d2c0-4df4-b4d9-2a9382a70bd8)

Since this CTF is titled "First Find" I will assume that we are meant to use the `find` command. This can be done with the following command `find / -name "uber-secret.txt" 2> /dev/null`. Broken down, 
everything before `2>` will find anywhere on the system where is a file (or directory) with that name. From the `2>` is telling the find command to ignore any possible permission errors, and since we 
are not running as a superuser we likely will run into many directories with locked permissions. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/3c908b12-2b0e-42f9-9b1b-4b2b8058dad5)

We can see that there is a bunch of nest directories that eventually contain the file we are looking for. Now if we take the output from that command, we can use `cat` to get the output of that file which turns out to 
be the flag. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/739b9b7b-5876-4777-8b80-a1a009af3542)
