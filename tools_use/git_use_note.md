###Git Use Note one

1. Create a github account

2. Install the git bash in own pc

3. plan and prepare your directory where store you github file

4. git initializtion
 * git config --global user.name "your github account name"
 * git config --global user.name "your github account sign up email"
 * After the two step, use the command 
> cat ~/.gitconfig
 * you will look the infomation of user

5. clone a repository
> git clone git@github.com:bellumpara/note.git


6. build ssh link to the github
 * Input the code
> $ssh-keygen -t rsa -C "youremail@example.com"

 * In your Adminstrator directory, there will have a .ssh folder. There are three file: 
   * id_rsa
   * id_rsa.pub 
   * known_hosts
 * copy the content of id_rsa.pub, and open the github account, find -->>setting -->>ssh key. 
 * click the add ssh key and paste the content into the ssh key. The title by yourself choice

7. create a folder
> mkdir note

 * Be sure you create the same name folder in the github

8. create a file
> touch readme.md

9. subl readme.md, add something

10. create the links from local folder to the github repository
> git remote add origin git@github.com:bellumpara/note.git
> git add <filename> (such as: readme.md)
> git commit -m "your comment"
> git push -u origin master

11. Above is the first time to use git. After, you just:
 * open the git bash in some directory
 * update the file from github to ensure online and offline same
>git pull 
 * operate, create file and content
>touch file
>git add file
>git commit -m "comment"
>git push origin master



