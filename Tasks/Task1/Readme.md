Pre-requisites
---------------

install python and pip

Install Fabric as well pip install fabric

fabric module will run by looking into fabfile.py

so create a fabfile.py as shown above

then run the below command

fab -H 10.25.84.10,15.25.84.11 -u ec2-user -i /tmp/Raja.pem remote_ex

here from the above command -H is for hostnames where we can specify as many as we can. 
And we can specify hostnames in file and send it to the above command as well .
-u is for Instruction of the User to login and execurte -i it will send the pem file path so that it can communicate to remote instances
