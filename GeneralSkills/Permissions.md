This is another simulation where it looks as though we will be changing the permissions on a file named `root`. 

Doing this, we must figure out how to gain access to the root directory as it is currently locked out. The attempts to change ownership of the directory via `chown` and `chmod` both do not allow us to edit permissions. 
We can now use `sudo -l` to check what we can access as a superuser as we cannot touch the root directory without it. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/8be01d20-372d-41bf-a752-86709c0c4444)

We can see we can access `/usr/bin/vi` which is a text editor where we may be able to enter a script to give us root access. Knowing that we have access to vi means we can search [GTFOBins](https://gtfobins.github.io/gtfobins/vi/) for a script to break out
of our permissions. 

In this file, without editing, the following was used `:!/bin/sh` to gain a root shell. Which immediately can be seen below that upon entering that command we have root access. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/b604d800-f988-4810-ac6c-c70141fc5e1d)

Now we just need to navigate to the root directory and find the root file to get the flag. Changing directories to root showed no visible files, but with a simple flag change to `-la` we can see there is some hidden files and one is notably titled ".flag.txt".
We can then `cat` to read this file and get the flag. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/77109a56-bab6-4df6-b3c6-de73853032b7)
