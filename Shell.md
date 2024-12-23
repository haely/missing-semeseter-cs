## Hello Shell: 
A shell is a command-line interpreter that allows you to interact with your computer's operating system by typing in commands.  Essentially, it acts as an intermediary between you and the operating system kernel.

### Types of Shell:
Just like there are different operating systems (Windows, macOS, Linux), there are different shells with varying features and strengths. Here are a few popular ones:   

**Bash (Bourne Again Shell)** 
This is the most common shell on Linux and macOS systems;  known for its wide range of features, scripting capabilities.   
**Zsh (Z Shell)**
Built upon Bash, offering enhanced features like plugins, themes, and improved auto-completion and 
**Others** 
PowerShell, Fish etc.

### Common Uses:

**System administration** 
Managing users, configuring network settings, automating system maintenance tasks.   
**Software development** 
Compiling code, running tests, managing version control systems.
**Data analysis**
Processing and analyzing large datasets, running statistical models.
**Everyday tasks** 
Managing files, Auromation etc.

## Some magical Tools (Mac specific): 
These are the tools that I install when I get a new mac. Get the latest versions from the official documents.
**iTerm**
Supercharged version of `terminal` the Mac default terminal. Helps split panes.
**Homebrew**
Mac (also Linux) package manager. Most tools, libraries can now be installed with a simple
`brew install <my_tool>`
and it's a picnic to update anything. 
**Zsh**
Only to get some cute cat themes for my terminal!
**Tmux**
Kind of like create different panes on one screen. Helps create persistent sessions, remote server management etc.

## Top Shell Commands

**Navigation:**

* `pwd` : Print Working Directory - shows your current location.
* `cd` : Change Directory.
    * `cd ..` : Move up one level.
    * `cd /` : Move to the root directory.
    * `cd ~` : Move to your home directory.
* `ls` : List Directory contents.
    * `ls -l` : Long listing format (more details).
    * `ls -a` : List all files, including hidden ones.

**File Management:**

* `touch <filename>` : Create an empty file.
* `mkdir <directoryname>` : Create a new directory.
* `cp <source> <destination>` : Copy files and directories.
* `mv <source> <destination>` : Move or rename files and directories.
* `rm <filename>` : Remove files and directories.
    * `rm -r <directoryname>` : Remove directories recursively.
    * `rm -f <filename>` : Force removal without prompting (use with caution!).
* `diff <file1> <file2>` : Differences between 2 files

**System Information:**

* `uname` : Display system information (kernel name, version, etc.).
* `df` : Disk Free - shows disk space usage.
* `du` : Disk Usage - shows file and directory space usage.
* `top` : Display real-time system processes.
* `free` : Display memory usage.

**Process Management:**

* `ps` : List running processes.
* `kill <processID>` : Terminate a process.
* `jobs` : List background jobs.
* `fg` : Bring a background job to the foreground.
* `bg` : Run a job in the background.

**Other Essentials:**

* `man <command>` : Manual - display the help page for a command.
* `grep <pattern> <filename>` : Search for a pattern in a file.
* `history` : List your recent commands.
* `history | grep <term>` : Recent commands containing the term.
* `find <directory> -name <filename>` : Locate files.
* `rg <searchterm>` : Recursive golbal search for a term. (Needs an install).
* `chmod <permissions> <filename>` : Change file permissions.
* `chown <user>:<group> <filename>` : Change file ownership.
* `|` (pipe) : Redirect output of one command to another.
* `>` : Redirect output to a file (overwrites existing content).
* `>>` : Append output to a file.
* `<` : Redirect input from a file.

## How to Create a Bash script
Bash scripting is a powerful way to automate tasks on Linux and macOS systems. Here's a step-by-step guide to get you started:

### 1. Create a new file

Use a text editor to create a new file. You can name it anything you like, but it's common to use a `.sh` extension (e.g., `my_script.sh`).

### 2. Add the shebang

The first line of your script should be the shebang: `#!/bin/bash`
This tells the system to use the Bash interpreter to execute the script.

### 3. Write your commands

Add the commands you want to execute, one per line. For example:

```bash
#!/bin/bash

echo "Hello, world!"
date
ls -l
```
### 4. Make the script executable

Use the `chmod` command for this
`chmod +x my_script.sh`

### 5. Run the script

`./my_script.sh`