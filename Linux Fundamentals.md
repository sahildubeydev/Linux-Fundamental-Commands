## Switch from windows to unbuntu

- `cd /mnt/c` : switch to c drive

## REPL

- Read, Evaluate, Print, Loop

## Note:

- For any Linux command you can check the usage and different input flags it expects by running the command followed by `--help`

## Commands

- `pwd` : this represents what is the current directory we are currently at.
- `ls` : you can print the content of the current directory we are in.
  - `ls -l` : lists down more details about file such as owner, permissions, date etc.
  - `ls -h` : works like `ls -l` but also gives size of the files
  - `ls -a` : also lists files and folders starting with `.`
- `cd` : this can help to move into a folder and move out of a folder.
  - `cd ..` : to jump one folder back from current direct ory
  - `cd ../..` : to jump two folder back from current directory and so on
  - `cd ~` : from any directory to come back to home directory
  - `cd directory1/directory2/` : to move into internal sub directories directly by separating them with a forward slash /

### Note:

- `cd ~` : tilda refers to the home directory.
- `cd /` : this slash leads to root directory
- **_Relative Path_** : It describes location of a file/folder w.r.t current folder
- **_Absolute Path_** : In this we mention the location from home directory or root directory

- `clear` : clears the working space by moving to the top of the current shell.
- `mkdir` : this helps us to create a new folder.
- `touch <filename>` : We can create a blank file.
- `cat > <filename>` : To write inside a file using linux terminal
- `cat <filename>` : prints the whole content of a file
- `cat /etc/passwd` : To list all users on linux and get id of users
- `rm <filename>` : this command deletes a file
- `rmdir <foldername>` : this command deletes an empty folder
- `rm -r <foldername>` : the -r flag enables rm to recursively delete all the content of the folder and then delete the folder
- `ls | grep python` : this pass the output of ls as an input to grep, grep does a substring search of python on the output of ls
- `ls > new.txt` : whatever is the result is it will be dumped into new.txt, nothing will be printed on the console. If new.txt has some content already then that will be replaced.
- `ls >> new.txt` : whatever is the result of is will be dumped into new.txt, nothing will be printed on the console. If new.txt has some content already then the new content will be appended.
- `<command 1> && <command 2>`: this executes command1 followed by command 2 considering command1 has no errors.
- `cp file1 file2` : copies the content of file1 to file2
- `cp -R /home/accounts/customers /home/accounts/vendors` : To copy a directory, including all its files and subdirectories, to another directory.
- `mv file1 file2` : moves(cut paste) the file1 to a new position as file2. This can also help us to rename a file.
- `tar -cf archive.zip 1.txt 2.txt` : this will add all the files mentioned after archive.zip into the zipped archive as mentioned.
- `tar -zcf archive1.zip 1.txt 2.txt` : this will add the file to the zip and also compress them.
- `tar xf archive1.zip -C extract` : all the content of the archive1 will be extracted out into the exact folder.
- `su <username>` : To change to a different user
- `ssh <username>@PORTNO` : To login a user to a port
- `wget <target file URL>` : To download a file from given URL
- `**cat /etc/os-release**` : To find OS name and version in Linux
- `rpm -qa` : List all installed packages in linux
- `sudo yum install -y <packagename>` : To install package in linux
- `sudo yum list installed` : To list all the installed packages
- `sudo yum remove -y <packagename>` : To uninstall package in linux
- `sudo yum install -y <packagename>-<version>` : To install package with desired version


## Vim

- `vim <filename>` : to create a file(if doesn't exist) and then open it in the vim editor in the normal mode. In normal mode we can't do changes to the file but we can read it and navigate it. We can also use `vi <filename>` to do the same. To go in insert mode press `i`. To come back press `esc`.
- `esc + :q` : To exit from a file.
- `esc + :q!` : To exit a file without saving changes
- `esc + :wq` : To exit a file with saving changes
- `l` : to move cursor to right
- `h` : to move cursor to left
- `j` : to move cursor down
- `k` : to move cursor up
- We can use normal right, left, up, down keys
- `dd` : in normal mode, it will delete the line the cursor is currently at.
- `gg` : It will move the cursor go on first line
- `G` : It will move cursor go on last line
- `w` : It will jump one word
- `2w` : It will jump two words
- `d2w` : It will delete 2 words
- `:%s/foo/bar/` : to replace all occurences of foo with bar
- `yw`: it copies one word
- `yy`: it copies whole line
- `p` : for pasting in normal mode
