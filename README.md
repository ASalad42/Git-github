# Git-github Week 2

## Git commands 
explain git commands: git init - git add - git commit - git push -u origin main - git pull

how to delete file/folder:
- rm -rf filename

## How to initlise repo on local host and make it available on github 
create repo online first

wite code > add changes > commit changes > push changes 

MAKE SURE IN CORRECT LOCATION AT ALL TIMES

Steps on localhost (assuming ssh connection established already):
mkdir filename
cd filename 
nano README.md > do edits then crl x to save then crl c to exist 
cat README.md 
git init 
git add README.md
git commit -m "message"
git branch -M main
git remote add origin git@github.com:ASalad42/eng122_week2.git
git push -u origin main (will work everytime as long in correct location)

*if permission denied add ssh key using agent (key in ssh folder so retrieve from there to establish connection again

## Pulling changes made on repo 
make changes on github globally 
git pull (make sure in correct folder)

## How to create repo on github and make it available on localhost
write code 
commit changes 
git clone 
