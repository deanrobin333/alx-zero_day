# Project 
** 0x03. Git
# Table of Contents
- [Author Details](#author-details)
- [Project Description](#project-description)
- [Tasks](#tasks)
	- [0. Create and setup your Git and GitHub account](#0)
---
## Author Details
- *Dean Robin Otsyeno - deanrobin777@gmail.com*

## Project Description
- At the end of this project you should be able to reproduce and understand these command lines:
```
$ git clone <repo>
$ touch test
$ git add test
$ git commit -m "Initial commit"
$ git push origin main
```
# Tasks
#### 0
**0. Create and setup your Git and GitHub account**
- Step 0 - Create an account on GitHub [if you do not have one already]
	- You will need a GitHub account for all your projects at ALX. If you do not already have a github.com account, you can create an account for free [here](https://github.com/)

- Step 1 - Create a Personal Access Token on Github
	- To have access to your repositories and authenticate yourself, you need to create a Personal Access Token on Github.

	- You can follow [this tutorial](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens) to create a token.
- Step 2 - Update your profile on the Intranet
- Step 3 - Create your first repository
	- Using the graphic interface on the github website, create your first repository.

		- Name: `alx-zero_day`
		- Description: `I'm now a ALX Student, this is my first repository as a full-stack engineer`
		- Public repo
		- No `README`, `.gitignore`, or license
- Step 4 - Open the sandbox
- Step 5 - Clone your repository

	- Clone your repository
	```
	root@896cf839cf9a:/# git clone https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/alx-zero_day.git                  
Cloning into 'alx-zero_day'...
warning: You appear to have cloned an empty repository.
	```
	- Replace {YOUR_PERSONAL_TOKEN} with your token from step 1

	- Replace {YOUR_USERNAME} with your username from step 0 and 1

	- Pro-Tip: On windows, use CTRL + A + V to paste in the web terminal

- Step 6 - Create the README.md and push the modifications
	- Navigate to this new directory.
	```
root@896cf839cf9a:/# cd alx-zero_day/
root@896cf839cf9a:/alx-zero_day#
	```
	- Create the file `README.md` with the content `My first readme`.
	```
root@896cf839cf9a:/alx-zero_day# echo 'My first readme' > README.md                                                                 
root@896cf839cf9a:/alx-zero_day# cat README.md                                                                                      
My first readme                                                                                             	```                          
	- Update your git identity
	```
root@896cf839cf9a:/alx-pre_course# git config --global user.email "you@example.com"
root@896cf839cf9a:/alx-pre_course# git config --global user.name "Your Name"
	```
	- Add this new file to git, commit the change with this message “My first commit” and push to the remote server / origin
	```
root@896cf839cf9a:/alx-zero_day# git add .
root@896cf839cf9a:/alx-zero_day# git commit -m 'My first commit'
[master (root-commit) 98eef93] My first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
root@896cf839cf9a:/alx-zero_day# git push                                                                                           
Enumerating objects: 3, done.                                                                                                         
Counting objects: 100% (3/3), done.                                                                                                   
Writing objects: 100% (3/3), 212 bytes | 212.00 KiB/s, done.                                                                          
Total 3 (delta 0), reused 0 (delta 0)                                                                                                 
To https://github.com/{YOUR_USERNAME}/alx-zero_day.git                                                                                       
 * [new branch]      master -> master              
	```



