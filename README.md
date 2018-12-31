# Github_Doc
Very short usefull reminder documentation for git and github use (Linux base)

Thank you to [Christophe](https://www.christopheducamp.com/2013/12/16/github-pour-nuls-partie-2/) for this. You can also vivit [git-handbook](https://guides.github.com/introduction/git-handbook/).

## Convention
Here after:
1. "Fn" sould be replaced by your filename
2. "Un" should be replaced by your username on github
3. "Pn" should be replaced by your projectname (github && local)
4. "Git_url" should be the url of the git repository (e.g. this https://github.com/PattyPTBS/Github_Doc)

## Very usefull git command to clone a github repository on your PC
- cd path/to/**root**_of_Pn_to_clone
- git clone Git_url

## Some usefull git commands on PC
- cd path/to/your/Pn
- git init
- git status
- git add Fn
- git commit -m "Add here a comment to describe your new commit"
- git commit -a -m "Add here a comment to describe your new commit"
- git remote add origin http<i></i>s://github.com/Un/Pn.git
- git remote -v
- git push

## Trick to visualize on your PC the mardown file README.md without need to push it into web site github.com/Un/Pn.git
On Linux, install pandoc which can convert a mardown file to a html file, and call it from e.g. firefox:
1. sudo apt install pandoc
2. cd path/to/your/Pn
3. pandoc -f mardown_github README.md -o README.html
4. firefox README.html

Point 3. and 4. could be replaced by a single command coded as follows (this use a temporary linux shared memory directory /dev/shm, sothat all is cleaned at reboot):

```bash
pdIn='README.md';pdOut=/dev/shm/${pdIn}.html;echo conversion $pdIn $pdOut;pandoc -f markdown_github $pdIn -o $pdOut;firefox $pdOut;rm $pdOut
```
