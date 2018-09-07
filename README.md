# devops-pipeline-chennai03sep2018

You will have to replace the authorized_keys file in ubuntu and centos folders with your public keys.

For example
============
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

5. If you would like to use this as local git repo then under the devops-pipeline-chennai03sep2018 folder,
you will have to delete .git folder with the command and create your own local repo.

rm -rf .git
git init
git config --global user.email "mail2jegan@gmail.com"
git config --global user.name "Jeganathan Swaminathan"
git add *
git commit -m "Initial commit."

You will have to replace the email id and name with your details :)

Now, issue pwd command to find the present working directory that can be used as git local repo.

pwd
/root/devops-pipeline-chennai03sep2018

In the case, the /root/devops-pipeline-chennai03sep2018 is your git local repo.

Enjoy DevOps!




