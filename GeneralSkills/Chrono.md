This is a simulation where we will be using SSH to connect to a box. Using the given credentials log into the account provided. Per the description we know that a `CronJob` runs at specified intervals. 
So the first step is to find where that directory may be. 

We start in the "PicoPlayer" directory which we have to back out of as it contains nothing. There is then a directory called "challenges" but permission is denied. As there are many directories and files here, some sort of command to 
find what we are looking for is needed.

Using the `find / -name "crontab" 2> /dev/null` commmand allows us to grab any locations where a crontab file might located without any errors. As per IBM "The crontab command submits, edits, lists, or removes cron jobs."

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/333c3e2b-8433-4520-a128-b3ee30adc9a5)

We know that the `/bin` directory contains binaries and probably will not be of use and using `cat` on this gives uninterpretable characters. When we `cat` on the other file we can see it displays the flag. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/41d5181f-0eef-46bd-a07a-39fc64513906)
