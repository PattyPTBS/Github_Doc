# Github_Doc
Very short usefull reminder documentation for git use

Thank you to [Christophe](https://www.christopheducamp.com/2013/12/16/github-pour-nuls-partie-2/) for this 

## Convention
Here after:
1. "Fn" sould be replaced by your filename
2. "Un" should be replaced by your username on github
3. "Pn" should be replaced by your projectname (github && local)

## Some usefull git commands
- cd path/to/your/Pn
- git init
- git status
- git add Fn
- git commit -m "Add here a comment to describe your new commit"
- git commit -a -m "Add here a comment to describe your new commit"
- git remote add origin https://<span></span>github.com/Un/Pn.git
- git remote -v
- git push

##Trick to visualize on your PC the mardown file README.md without need to push it to github.com/Un/Pn.git
On Linux, install pandoc which can convert a mardown file to a html file, and call it from e.g. firefox:
1. sudo apt install pandoc
2. cd path/to/your/Pn
3. pandoc -f mardown_github README.md -o README.html
4. firefox README.html
