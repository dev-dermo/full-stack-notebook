# Full Stack Notebook

## Golden Rules
* **No spaces** in file, folder, or repo names
* Pay attention to and match letter/word casing 
* Always `pull` before `push` (when working collaboratively)
* Commit early, commit often

## Command line/terminal operations:

* To print out current working directory:
```
pwd
```

* To print out the contents of the current directory: `ls`, can be expanded with more information using the `-la` flags:
```
ls -la
```

* To change directory:
```
cd /path/to/folder
```

* `~` refers to the "home" directory
* `.` refers to the "current" directory
* `..` refers to the "parent" directory, example usage: `cd ..` to go up one level



## Basic Git

First create repo on GitHub, then in a directory that makes sense such as "/coding-bootcamp-projects", run:
```
git clone git@github.com:diarmuid-murphy/full-stack-notebook.git
``` 

> N.B. Note that the url in the above snippet will vary per repo. 

> N.B. Also note that cloning a repo is the process of getting a copy on your machine and only needs to be done once. To get updates from a repo, run `git pull`.

Once you have the repo on you machine, change into that directory using `cd`

Finally, from within the repo you can run the following commands each time you want to make a "save".

```
git add -A OR git add .
git commit -m "a descriptive label for your commit"
git push
```

<!-- ## Common Errors

* Off by one error eg, `i = 1` vs `i = 0`
* Pluralization/casing eg. `Console.log()` vs `console.log()` or `student` vs `students`
* Wrong/unexpected data types, use `typeof` to confirm data type -->