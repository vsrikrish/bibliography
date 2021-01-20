# bibliography

This repository contains `.bib` files containing my papers. 
* `my-papers.bib`: papers by me;

## Use

I use this in my [group's website](https://github.com/srikrishnan-lab/srikrishnan-lab.github.io) as well as my [CV](https://github.com/vsrikrish/cv) as a [`git` submodule](https://www.vogella.com/tutorials/GitSubmodules/article.html). Pushing an update triggers rebuilding the website and CV.

### Add to Project

To add to a project, use:
```
git submodule add -b main https://github.com/vsrikrish/bibliography.git
git submodule init
```  
To pull the latest updates:
```
git submodule update
cd bibliography
git pull
cd ..
```
And to remove:
```
# remove the submodule entry from .git/config
git submodule deinit -f bibliography

# remove the submodule directory from the superproject's modules directory
rm -rf .git/modules/bibliography

# remove the entry in .gitmodules and remove the submodule directory
git rm -f bibliography
```
