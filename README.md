# FiveAtoms
A set of Python programs for console user-ability

The default logins are below:

Master account:
Username: admin
Password: admin

Regular account:
Username: hello
Password: hello

***When logging in to the master account, a PIN is generated and stored in auth.json. This changes everytime to simulate 2FA. 

Below we'll explain some of the files and their functions:

Main.py -- This is the main login and account settings file. You login to it by entering a regular username and regular password,
or by entering a master username, master password, and 6-digit code generated by auth.py.

Auth.py -- This is the Python program that contains the functions to generate and then store the 6-digit pin in auth.json

Encode.py -- This is the file for you to use to create your own passwords and then put them in master_password.json and password.json 
respectively. Run this program and enter a regular password and it returns what you input and the hashed form. Take the hashed form and 
put them into the two password JSON files.

Check.py -- This is a file-in-the-making that would check if there is a stored password for either account, and then offer to create a 
password.

The various JSON files -- These are used for dynamic settings, like password changes and username changes.
