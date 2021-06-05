# Full Stack Notebook

## Golden Rules
* **No spaces** in file, folder, or repo names
* Pay attention to and match letter/word casing 
<!-- * Always `pull` before `push` (when working collaboratively) -->
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

## SSH Keys

> Used to authenticate your computer without having to enter a password over and over.

### On MacOS, first run:
```
ssh-keygen -t rsa
```

Followed by: 
```
pbcopy < ~/.ssh/id_rsa.pub
```

This places your SSH key onto your clipboard, now go to GitHub, and under `Settings>SSH and GPG keys` paste this new SSH key.

### On Windows, first run:
```
ssh-keygen -o
```

Followed by:
```
cat ~/.ssh/id_rsa.pub
```

This will print out your SSH key which you will manually need to highlight and copy to your clipboard.

Example output: 
```
ssh-rsa AAAAB3NzaC1yc2EAAAABIwAAAQEAklOUpkDHrfHY17SbrmTIpNLTGK9Tjom/BWDSU
GPl+nafzlHDTYW7hdI4yZ5ew18JH4JW9jbhUFrviQzM7xlELEVf4h9lFX5QVkbPppSwg0cda3
Pbv7kOdJ/MTyBlWXFCR+HAo3FXRitBqxiX1nKhXpHAZsMciLq8V6RjsNAQwdsdMFvSlVK/7XA
t3FaoJoAsncM1Q9x5+3V0Ww68/eIFmb1zuUFljQJKprrX88XypNDvjYNby6vw/Pb0rwert/En
mZ+AW4OZPnTPI89ZPmVMLuayrD2cE86Z/il8b+gw3r3+1nKatmIkjn2so1d01QraTlMqVSsbx
NrRFi9wrf+M7Q== schacon@mylaptop.local
```

Finally, go to GitHub, and under `Settings>SSH and GPG keys` paste this new SSH key.

## Basic Git

### Making a Repo on GitHub, 3 important steps
1. Enter a repo name, with no spaces
2. Make sure repo is set to "Public"
3. Click the option to add a README.md file - ***this will make your life much easier!!!***

First create repo on GitHub, then on your machine, in a directory that makes sense such as "/coding-bootcamp-projects", run:
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

<!-- https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line -->

<!-- https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal -->