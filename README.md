devops-kubernetes-practical-01
make the clustering of 3 nodes and create ngnix deployment of of 3 replica
Basic

Own Security group, that allow all traffic from any destinatin to Ec2 machine
Create 3 instance ( t2. mediaum / ubuntu latest ami) with common keypair
Attach instances with security group , that create in step 1
Rename all the machine as master, slave1 & slave2
Setup of master machine -

Access the master machine by putty or any other tools

Take the administrative previlege by command : sudo su

change the host name by command : hostnamectl set-hostname master # for master its master , for slave 1 its savel1 like this .

create a file install.sh and paste the command from the link and save it Link - link

execute the file the command is : bash install.sh

do the same activities (1-4) all the 3 nodes

do the cluster setup the command is : kubeadm init # this command will through the token for all save1 and salve2

