# Git-github Week 2
Git is the industry standard version control system for developers 

## Git diagram 
![image](https://user-images.githubusercontent.com/104793540/182138775-002d35d4-f184-4f3d-881b-1ca198527334.png)


## Git commands 

- Git init > Create an empty Git repository or reinitialize an existing one
- Git add > add files from working area to staging area (index?)
- Git status > inspects contents of working direcotry 
- Git commit > perm stores file changes from staging area in repo 
- Git push > push to remote repo 
- Git pull > Fetch from and integrate with another repository or a local branch (pull latest from remote repo)
- Git clone >  Clone a repository into a new directory
- Git log > show commit logs 
- Git diff >  Show changes between commits, commit and working tree, etc
- Git branch >  List, create, or delete branches

how to delete file/folder:
- rm -rf filename

## How to initlise repo on local host and make it available on github 
create repo online first
wite code > add changes > commit changes > push changes 
MAKE SURE IN CORRECT LOCATION AT ALL TIMES
Steps on localhost (assuming ssh connection established already):
- mkdir filename
- cd filename 
- nano README.md > do edits then crl x to save then crl c to exist 
- cat README.md 
- git init 
- git add README.md
- git commit -m "message"
- git branch -M main
- git remote add origin git@github.com:ASalad42/eng122_week2.git
- git push -u origin main (will work everytime as long in correct location)

*if permission denied add ssh key using agent (key in ssh folder so retrieve from there to establish connection again)

### If you dont have ssh keys setup do the following 
- create .ssh directory (folder) mkdir .ssh
- open directory with cd. ssh
- Generate key with $ssh-keygen -t rsa -b 4096 -C "youremail@example.com"
- Email MUST be the same as your github account
- you will then be prompted to enter a file name and a passphrase
- upon completion, you will get a public and private key
- copy the .pub and paste into github (settings>ssh and gpg keys section)
- once connection establish you can git push 


## Pulling changes made on repo 
- make changes on github globally 
- git pull (make sure in correct folder)

## How to create repo on github and make it available on localhost
- create new repo including readme file 
- write code in readme file 
- commit changes 
- on local host create an empty folder 
- mkdir filename
- cd filename
- git clone 
