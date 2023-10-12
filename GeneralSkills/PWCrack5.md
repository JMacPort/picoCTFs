We will again grab all of the necessary files, this time being four, with one being a dictionary. 

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/bb52640f-446d-48bb-ab9e-f117c8b8e374)

Per usual, we will read each file and display the outputs below. 
![image](https://github.com/JMacPort/picoCTFs/assets/145376972/d7a0a80e-6b51-4ba6-bc93-0f93662b57bc)
![image](https://github.com/JMacPort/picoCTFs/assets/145376972/30a0ed90-e9d6-4d13-9f7d-a17c7aec293b)
![image](https://github.com/JMacPort/picoCTFs/assets/145376972/c4e1d7b9-6d61-47f2-8c31-abea180120e5)
![image](https://github.com/JMacPort/picoCTFs/assets/145376972/724f9df5-8f70-41c0-a5ab-7465c579f492)

We can see the dictionary includes many strings which will be used to discover the password, the hash and flag both do not provide any useful information and the `level5.py` script is very similar to the last which means the same methods may work.

Now we should create another python function similar to the last except we will be used the possible passwords in a variable as now we can open it. The python file is shown below.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/753396a3-89af-404f-926c-83dde6e0d4a3)

The difference between this script and last script is very minimal. Now the passwords are opened and stored in a variable called `list_of_pw` and reads each line. Then in the `for` loops each password containts additional whitespace so the 
strip method is used and then stored each possible password in `pos_pass`. We then call the `hash_pw` function on each possible password and compare to see if it is equal to `correct_pw_hash`. This will give us the password used to access the flag.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/ac974c05-1a66-4d6e-b515-57a1ded49ea0)

Entering this password in the `level5.py` script gives us our flag.

![image](https://github.com/JMacPort/picoCTFs/assets/145376972/58f2e806-f807-4939-b92a-facf980c3a3d)
