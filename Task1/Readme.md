
Assignment 2:

Write a bash/python script that takes list of hostnames (comma separated) as an argument.

This script, when executed, should connect to all the servers via. SSH (standard port) (assume password-less connectivity) and give a single prompt to the user.

When the user executes a command on this prompt, the script should run the command on all connected servers and display the output.

Make this as efficient as possible, code comments appreciated.

Pre-requisites
---------------

install python 2.7.5 and pip

Install Fabric as well pip install fabric

fabric module will run by looking into fabfile.py

so create a fabfile.py as shown above

then run the below command

fab -H 10.25.84.10,15.25.84.11 -u ec2-user -i /tmp/Raja.pem remote_ex

here from the above command -H is for hostnames where we can specify as many as we can. 
And we can specify hostnames in file and send it to the above command as well .
-u is for Instruction of the User to login and execurte -i it will send the pem file path so that it can communicate to remote instances
