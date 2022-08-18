# Accessing-server-to-server


- first need to edit in vi /etc/ssh/sshd_config
- password authentication yes
- systemctl restart sshd
- then set password for the both servers
- then genrate ssh keys in the admin server
- ssh-keygen
- then push into the server 2 for access
- ssh-copy-id ec2-user@<private-ip>
- it asking the password for the server 2
- enter the password 
- then ssh ec2-user@<private-ip>
- now you can acces the server 2 in the admin server
