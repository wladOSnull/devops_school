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

> ***Linux git main***  
1 - git clone "ssh URL of origin repo"  
2 - cd devops_school  
3 - ls -l  
4 - cp -a ~/Documents/hw3/. ./  
5 - ls -a  
6 - git add -A  
7 - git ls-files  
8 - git commit -a -m "add: added all existed files from hw3"  
9 - git push origin main  
10 - git log / git log --oneline  

> ***Linux git new_branch***  
1 - git status  
2 - git branch new_branch  
3 - git branch  
4 - git checkout new_branch  
5 - git branch -a  
6 - git status  

> ***Linux git new_branch new file***  
1 - touch bash_nb.sh  
2 - git add bash_nb.sh   
3 - git commit -a -m "add and edit: added new empty sh file and edited info.txt"  
4 - nano info.txt  
5 - git status  
6 - git push origin new_branch  

> ***Linux git new_branch edit file***  
1 - nano bash_nb.sh  
2 - nano info.txt  
3 - git status  
4 - git commit -a -m "edit: changed pattern into  bash_nb.sh and edited info.txt"  

> ***Linux git main merge new_branch***  
1 - git checkout main  
2 - git branch  
3 - git merge new_branch  
4 - git pull origin main  
5 - git push origin main  

> ***Linux git final***  
git log --oneline --decorate --graph --all  
![git_result](https://user-images.githubusercontent.com/29982996/144261260-93831bc7-a612-4537-9a54-06726a3774e8.png)
