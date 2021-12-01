# Ch DevOps School 2021
### Git/GitFlow lesson
---


> ***Linux***  
1 - sudo apt install git  
2 - ssh-keygen -t rsa -b 4069 -C my@mail.com (create passphrase)  
3 - copy public key from id_rsa.pub  

> ***GitHub***  
1- create new ssh key with public key from id_rsa.pub   

> ***Linux***  
1 - eval "$(ssh-agent -s)"  
2 - ssh-add ~/.ssh/id_rsa (input passphrase)  
3 - ssh -T git@github.com (input passphrase)  
4 - cd ~/Documents  
5 - mkdir repo1  
6 - cd repo1  
7 - git clone "ssh URL of origin repo"  
8 - cd devops_school  
9 - ls -l  
10 - cp -a ~/Documents/hw3/. ./  
11 - ls -a  
12 - git add -A  
13 - git ls-files  
14 - git commit -a -m "add: added all existed files from hw3"  
15 - git push origin main  
