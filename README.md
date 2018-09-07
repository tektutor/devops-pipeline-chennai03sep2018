# devops-pipeline-chennai03sep2018

You will have to replace the authorized_keys file in ubuntu and centos folders with your public keys.

For example
++++++++++++

1. Clone the git repository with the below command in Linux terminal or Windows command prompt
git clone tektutor/devops-pipeline-chennai03sep2018.git

2. Switch to devops-pipeline-chennai03sep2018 folder
cd devops-pipeline-chennai03sep2018

3. Now generate key the Public/Private keys using the below command
ssh-keygen

4. Now copy the public key to ubuntu and centos folders as shown below
cp /root/.ssh/id_rsa.pub ubuntu/authorized_keys
cp /root/.ssh/id_rsa.pub centos/authorized_keys

My assumption is you have logged in as root in the terminal.

