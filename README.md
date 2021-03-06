# mac-env
my local env setup for Mac. including shell cli short cut. brew package ..

------------

### SHORTCUTS

| Key/Command | Description |
| ----------- | ----------- |
| Ctrl + A   | Go to the beginning of the line you are currently typing on.  This also works for most text input fields system wide.  Netbeans being one exception |
| Ctrl + E   | Go to the end of the line you are currently typing on.  This also works for most text input fields system wide.  Netbeans being one exception |
| Ctrl + Q   | Clears the line |
| Ctrl + L   | Clears the Screen |
| Cmd + K    | Clears the Screen |
| Ctrl + U   | Cut everything backwards to beginning of line |
| Ctrl + K   | Cut everything forward to end of line |
| Ctrl + W   | Cut one word backwards using white space as delimiter |
| Ctrl + Y   | Paste whatever was cut by the last cut command |
| Ctrl + H   | Same as backspace |
| Ctrl + C   | Kill whatever you are running.  Also clears everything on current line |
| Ctrl + D   | Exit the current shell when no process is running, or send EOF to a the running process |
| Ctrl + Z   | Puts whatever you are running into a suspended background process. fg restores it |
| Ctrl + _   | Undo the last command. (Underscore.  So it's actually Ctrl + Shift + minus) |
| Ctrl + T   | Swap the last two characters before the cursor |
| Ctrl + F   | Move cursor one character forward |
| Ctrl + B   | Move cursor one character backward |
| Option + →  | Move cursor one word forward |
| Option + ←  | Move cursor one word backward |
| Esc + T  | Swap the last two words before the cursor |
| Esc + Backspace | Cut one word backwards using none alphabetic characters as delimiters |
| Tab  | Auto-complete files and folder names |

### CORE COMMANDS

| Key/Command | Description |
| ----------- | ----------- |
| cd [folder] | Change directory e.g. `cd Documents` |
| cd |  Home directory |
| cd ~ |  Home directory |
| cd /  | Root of drive |
| cd -  | Previous directory |
| ls | Short listing |
| ls -l | Long listing |
| ls -a | Listing incl. hidden files |
| ls -lh| Long listing with Human readable file sizes |
| ls -R | Entire content of folder recursively |
| sudo [command] | Run command with the security privileges of the superuser (Super User DO) |
| open [file] | Opens a file ( as if you double clicked it ) |
| top | Displays active processes. Press q to quit |
| top -ocpu -s 5 | Displays active processes by cpu 5s time intervel . Press q to quit |
| lsof -i | grep ESTABLISHED | Displays TCP connection |

| nano [file] | Opens the file using the nano editor |
| vim [file] | Opens the file using the vim editor |
| clear |  Clears the screen |
| reset |  Resets the terminal display |

### CHAINING COMMANDS

| Key/Command | Description |
| ----------- | ----------- |
| [command-a]; [command-b] | Run command A and then B, regardless of success of A |
| [command-a] && [command-b] | Run command B if A succeeded |
| [command-a] \|\| [command-b] | Run command B if A failed |
| [command-a] & | Run command A in background |


### PIPING COMMANDS

| Key/Command | Description |
| ----------- | ----------- |
| [command-a] \| [command-b] | Run command A and then pass the result to command B e.g ps auxwww \| grep google |


### COMMAND HISTORY

| Key/Command | Description |
| ----------- | ----------- |
| history n |  Shows the stuff typed – add a number to limit the last n items |
| Ctrl + r  | Interactively search through previously typed commands |
| ![value] |  Execute the last command typed that starts with ‘value’ |
| ![value]:p |  Print to the console the last command typed that starts with ‘value’ |
| !! |  Execute the last command typed |
| !!:p |  Print to the console the last command typed |

### FILE MANAGEMENT

| Key/Command | Description |
| ----------- | ----------- |
| touch [file] |   Create a new file |
| pwd | Full path to working directory |
| . |  Current folder, e.g. `ls .` |
| .. | Parent/enclosing directory, e.g. `ls ..` |
| ls -l .. | Long listing of parent directory |
| cd ../../ | Move 2 levels up |
| cat | Concatenate to screen |
| rm [file] |  Remove a file, e.g. `rm data.tmp` |
| rm -i [file] | Remove with confirmation |
| rm -r [dir] | Remove a directory and contents |
| rm -f [file] | Force removal without confirmation |
| cp [file] [newfile] | Copy file to file |
| cp [file] [dir] | Copy file to directory |
| mv [file] [new filename] |  Move/Rename, e.g. `mv file1.ad /tmp` |
| pbcopy < [file] | Copies file contents to clipboard |
| pbpaste | Paste clipboard contents |
| pbpaste > [file] | Paste clipboard contents into file, `pbpaste > paste-test.txt` |

### DIRECTORY MANAGEMENT

| Key/Command | Description |
| ----------- | ----------- |
| mkdir [dir] | Create new directory |
| mkdir -p [dir]/[dir] |  Create nested directories |
| rmdir [dir] | Remove directory ( only operates on empty directories ) |
| rm -R [dir] | Remove directory and contents |
| less [file]|  Output file content delivered in screensize chunks |
| [command] > [file] |  Push output to file, keep in mind it will get overwritten |
| [command] >> [file] | Append output to existing file |
| [command] < [file] |  Tell command to read content from a file |

### SEARCH

| Key/Command | Description |
| ----------- | ----------- |
| find [dir] -name [search_pattern] | Search for files, e.g. `find /Users -name "file.txt"` |
| grep [search_pattern] [file] | Search for all lines that contain the pattern, e.g. `grep "Tom" file.txt` |
| grep -r [search_pattern] [dir] | Recursively search in all files in specified directory for all lines that contain the pattern |
| grep -v [search_pattern] [file] | Search for all lines that do NOT contain the pattern |
| grep -i [search_pattern] [file] | Search for all lines that contain the case-insensitive pattern |
| mdfind [search_pattern] | Spotlight search for files (names, content, other metadata), e.g. `mdfind skateboard` |
| mdfind -onlyin [dir] -name [pattern] | Spotlight search for files named like pattern in the given directory |

### HELP

| Key/Command | Description |
| ----------- | ----------- |
| [command] -h |  Offers help |
| [command] --help | Offers help |
| info [command] | Offers help |
| man [command] |  Show the help manual for [command] |
| whatis [command] | Gives a one-line description of [command] |
| apropos [search-pattern] | Searches for command with keywords in description |

### GIT

### Glossary

| Keywords                     | Description                                                                                                             |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| git                          | Open-source distributed version-control system, used to store code in repositories                                      |
| GitHub, GitLab and Bitbucket | Platform for hosting and collaborating on Git repositories                                                              |
| staging                      | Proposed files/directories that you'd like to commit                                                                    |
| commit                       | Saving all staged files/directories to your local repository                                                            |
| branch                       | An independent line of development, so you can develop features isolated from each other. Master branch is the default. |
| clone                        | Local version of a repository, including all commits and branches                                                       |
| remote                       | Common repository on eg. Github that all team members to keep that changes in sync with                                 |
| fork                         | Copy of a repository owned by a different user                                                                          |
| pull request                 | A method of submitting contributions to a repository                                                                    |
| HEAD                         | Represents your current working directory                                                                               |

### Configuration

| Key/Command                              | Description                                         |
| ---------------------------------------- | --------------------------------------------------- |
| `git config --global user.name [name]`   | Set author name to be used for all commits          |
| `git config --global user.email [email]` | Set author email to be used for all commits         |
| `git config color.ui true`               | Enables helpful colorization of command line output |

### Core Commands

| Key/Command                 | Description                                              |
| --------------------------- | -------------------------------------------------------- |
| `git init [directory]`      | Creates new local repository                             |
| `git clone [repo]`          | Creates local copy of remote repository                  |
| `git add [directory]`       | Stages specific [directory]                              |
| `git add [file]`            | Stages specific [file]                                   |
| `git add -A`                | Stages all changed files                                 |
| `git add .`                 | Stages new and changed files, NOT deleted files          |
| `git add -u`                | Stages changed and deleted files, NOT new files          |
| `git commit -m "[message]"` | Commit everything that is staged                         |
| `git status`                | Shows status of changes as untracked, modified or staged |

### Synchronization of Changes

| Key/Command   | Description                                                                           |
| ------------- | ------------------------------------------------------------------------------------- |
| `git fetch`   | Downloads all history from the remote branches                                        |
| `git merge`   | Merges remote branch into current local branch                                        |
| `git pull`    | Downloads all history from the remote branch and merges into the current local branch |
| `git push`    | Pushes all the commits from the current local branch to its remote equivalent         |

*Tip: `git pull` is the combination of `git fetch` and `git merge`*

### Undo Changes

| Key/Command                 | Description                                                                                 |
| --------------------------- | ------------------------------------------------------------------------------------------- |
| `git checkout -- [file]`    | Replace file with contents from HEAD                                                        |
| `git revert [commit]`       | Create new commit that undoes changes made in [commit], then apply it to the current branch |
| `git reset [file]`          | Remove [file] from staging area                                                             |
| `git reset --hard HEAD`     | Removes all local changes in working directory                                              |
| `git reset --hard [commit]` | Reset your HEAD pointer to previous commit and discard all changes since then               |

### Branches

| Key/Command                | Description                        |
| -------------------------- | ---------------------------------- |
| `git branch [branch]`      | Create a new branch                |
| `git checkout [branch]`    | Switch to that branch              |
| `git checkout [branch] -b` | Create and checkout new branch     |
| `git merge [branch]`       | Merge [branch] into current branch |
| `git branch -d [branch]`   | Deletes the [branch]               |
| `git push origin [branch]` | Push [branch] to remote            |
| `git branch`               | Lists local branches               |
| `git branch -r`            | Lists remote branches              |
| `git branch -a`            | Lists local and remote branches    |

### History

| Key/Command                | Description                                                      |
| -------------------------- | ---------------------------------------------------------------- |
| `git log`                  | Lists version history for the current branch                     |
| `git log --author=[name]`  | Lists version history for the current branch from certain author |
| `git log --oneline`        | Lists compressed version history for the current branch          |
| `git show [commit]`        | Outputs metadata and content changes of the specified commit     |
| `git blame [file]`         | Shows who changed what and when in file                          |
