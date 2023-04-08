# Introduction to Linux

## Objectives
* Create and manipulate folders and files
* Create and manage permissions, security, and services
* Some helpful commands

## Create and manipulate folders and files

### ls
`ls` is a command used in Unix-like operating systems to list the files and directories in a given directory.

1. To list the contents of the current directory:

    ``` bash
    ls
    ```

2. To list the contents of a specific directory:

    ``` bash
    ls /path/to/directory
    ```

3. To list the contents of a directory in long format (displays more information about each file):

    ``` bash
    ls -l /path/to/directory
    ```
    
4. To list the contents of a directory including hidden files:
    ``` bash
    ls -a /path/to/directory
    ```

### mkdir
`mkdir` is a command used in Unix-like operating systems to create a new directory. It stands for "make directory." You can use it to create a new directory in the current directory or to create a new directory with a specified path.

1. To create a new directory in the current directory:

    ``` bash
    mkdir new_directory
    ```

2. To create a new directory with a specified path:

    ``` bash
    mkdir /path/to/new_directory
    ```

3. To create a new directory with multiple nested directories:

    ``` bash
    mkdir -p /path/to/new_directory/nested_directory/subdirectory
    ```
    > Note: The -p option creates all the directories in the specified path, even if some of the parent directories do not exist.

4. To create multiple directories at once:

    ``` bash
    mkdir directory1 directory2 directory3
    ```
    
    > Note: This will create three directories named "directory1," "directory2," and "directory3" in the current directory.


### cd
`cd` is a command used in Unix-like operating systems to change the current working directory. It stands for "change directory." You can use it to navigate to a different directory in the file system.

1. To change to the home directory:
    ``` bash
    cd
    ```

2. To change to a specific directory:
    ``` bash
    cd /path/to/directory
    ```

3. To change to the parent directory:
    ``` bash
    cd ..
    ```

4. To change to the previous directory:
    ``` bash
    cd -
    ```
    > Note: This will switch to the previous directory you were in.

5. To change to a directory using a relative path:
    ``` bash
    cd path/to/directory
    ```
    > Note: This will change to a directory relative to the current working directory.


### touch
`touch` is a command used in Unix-like operating systems to create an empty file or update the timestamp of an existing file. It stands for "touch file." You can use it to create a new file or update the modification time of an existing file without changing its content.

1. To create a new empty file:
    ``` bash
    touch filename.txt
    ```
    > Note: This will create an empty file named "filename.txt" in the current directory.



2. To create multiple files at once:
    ``` bash
    touch file1.txt file2.txt file3.txt
    ```
    > Note: This will create three empty files named "file1.txt," "file2.txt," and "file3.txt" in the current directory.


    
3. To update the modification time of a file to a specific time:
    ``` bash
    touch -t 202201010101.01 filename.txt
    ```
    > Note: This will update the modification time of the file "filename.txt" to January 1, 2022, at 1:01:01.01 AM.


### git
`git` is a command-line tool used for version control in software development. It allows developers to track changes to source code over time, collaborate with others on the same project, and revert to earlier versions of the code if necessary. With Git, you can create branches to experiment with new features, merge changes from different branches, and manage the history of the codebase.

1. To initialize a new Git repository:
    ``` bash
    git init
    ```
    > Note: This will create a new Git repository in the current directory.



2. To add files to the staging area:
    ``` bash
    git add filename.txt
    ```
    > Note: This will add the file "filename.txt" to the staging area, which is where you prepare changes to be committed.


3. To commit changes to the repository:
    ``` bash
    git commit -m "Commit message"
    ```
    > Note: This will commit the changes in the staging area to the repository with a message describing the changes.


4. To create a new branch:
    ``` bash
    git branch new-branch
    ```
    > Note: This will create a new branch named "new-branch" based on the current branch.



5. To switch to a different branch:
    ``` bash
    git checkout branch-name
    ```
    > Note: This will switch to the branch named "branch-name."



6. To merge changes from one branch into another:
    ``` bash
    git merge branch-name
    ```
    > Note: This will merge the changes from the branch named "branch-name" into the current branch.



### nano
`nano` is a command-line text editor for Unix-like operating systems. It allows users to create and edit text files in the terminal. With nano, you can create new files, open existing files, make changes to text, and save the changes. It is a beginner-friendly editor that is easy to use and learn.

1. To create a new file:
    ``` bash
    nano filename.txt
    ```
    > Note: This will open a new file named "filename.txt" in the nano editor.

2. This will open a new file named "filename.txt" in the nano editor.
    ``` bash
    nano existing_file.txt
    ```
    > Note: This will open the existing file named "existing_file.txt" in the nano editor.

3. To make changes to the text:
    ``` text
    Use the arrow keys to move the cursor to the location where you want to make changes. 
    Type in the text that you want to add or delete.
    ```
    
4. To save changes:
    ``` text
    Press `Ctrl+O` to save changes to the file. Press `Ctrl+X` to exit nano.
    ```

5. To search for text:
    ``` text
    Press `Ctrl+W` to search for text within the file. 
    Type in the text you want to search for and press `Enter`.
    ```

6. To cut, copy, and paste text:
    ``` bash
    Use the `Alt+6` shortcut to cut text, 
    `Alt+u` to undo, 
    `Alt+0` to copy text, 
    and `Alt+e` to paste text.
    ```

### vim
`vim` is a command-line text editor for Unix-like operating systems. It allows users to create and edit text files in the terminal. With vim, you can create new files, open existing files, make changes to text, and save the changes. It is a powerful and customizable editor that can be used efficiently with keyboard shortcuts. It is widely used by developers and system administrators.

1. To create a new file:
    ``` bash
    vim filename.txt
    ```
    > Note: This will open a new file named "filename.txt" in the vim editor.

2. To open an existing file:
    ``` bash
    vim existing_file.txt
    ```
    > Note: This will open the existing file named "existing_file.txt" in the vim editor.

3. To make changes to the text:
    ``` text
    Use the arrow keys to move the cursor to the location where you want to make changes. 
    Type in the text that you want to add or delete.
    ```

4. To save changes:
    ``` text
    Press `Esc` to enter command mode, then type `:w` and press `Enter` to save changes to the file.
    Type `:q` and press `Enter` to quit vim.
    ```

5. To search for text:
    ``` text
    Press `/` to enter search mode. 
    Type in the text you want to search for and press `Enter`. 
    Use `n` to go to the next match, and `N` to go to the previous match.
    ```

6. To cut, copy, and paste text:
    ``` text
    Use `dd` to cut a line, `yy` to copy a line, and `p` to paste a line.
    ```

### cp
`cp` is a command used in Unix-like operating systems to copy files or directories. It allows users to create a duplicate copy of an existing file or directory. The basic syntax of the `cp` command is `cp source destination`. The `source` parameter is the file or directory that you want to copy, and the `destination` parameter is where you want to copy the file or directory to.

1. To copy a file to another location:
    ``` bash
    cp file.txt /path/to/destination/
    ```
    > Note: This will copy the file "file.txt" to the specified destination directory.

2. To copy a file and rename it:
    ``` bash
    cp file.txt newfile.txt
    ```
    > Note: This will create a copy of "file.txt" with the new name "newfile.txt" in the same directory.

3. To copy a directory and its contents:
    ``` bash
    cp -r directory/ /path/to/destination/
    ```
    > Note: This will copy the directory "directory" and its contents to the specified destination directory.

4. To overwrite an existing file:
    ``` bash
    cp -f source_file.txt destination_file.txt
    ```
    > Note: This will copy the file "source_file.txt" to "destination_file.txt", overwriting it if it already exists. The -r option is used to copy directories recursively, and the -f option is used to force overwriting of existing files without prompting for confirmation.


### mv
`mv` is a command used in Unix-like operating systems to move or rename files and directories. It allows users to change the location or name of an existing file or directory. The basic syntax of the `mv` command is `mv source destination`. The `source` parameter is the file or directory that you want to move or rename, and the `destination` parameter is where you want to move or rename the file or directory to.

1. To move a file to another location:
    ``` bash
    mv file.txt /path/to/destination/
    ```
    > Note: This will move the file "file.txt" to the specified destination directory.

2. To rename a file:
    ``` bash
    mv oldname.txt newname.txt
    ```
    > Note: This will rename the file "oldname.txt" to "newname.txt" in the same directory.

3. To move a directory and its contents:
    ``` bash
    mv directory/ /path/to/destination/
    ```
    > Note: This will move the directory "directory" and its contents to the specified destination directory.

4. To overwrite an existing file:
    ``` bash
    mv -f source_file.txt destination_file.txt
    ```
    Note: This will move the file "source_file.txt" to "destination_file.txt", overwriting it if it already exists. The `-f` option is used to force overwriting of existing files without prompting for confirmation.




### cat
`cat` is a command used in Unix-like operating systems to display the contents of a file on the terminal. It allows users to view the content of one or more files in their entirety. The basic syntax of the cat command is cat file1 file2 file3. The file1, file2, and file3 parameters represent the names of the files that you want to view the contents of.

1. To display the contents of a single file:
    ``` bash
    cat file.txt
    ```
    Note: This will display the contents of the file "file.txt" on the terminal.

2. To concatenate multiple files into one file:
    ``` bash
    cat file1.txt file2.txt > combined.txt
    ```
    Note: This will concatenate the contents of "file1.txt" and "file2.txt" into a new file named "combined.txt".

3. To display the contents of a file with line numbers:
    ``` bash
    cat -n file.txt
    ```
    Note: This will display the contents of the file "file.txt" on the terminal with line numbers added to each line.

4. To display the contents of a file and scroll through it:
    ``` bash
    cat file.txt | less
    ```
    Note: This will display the contents of the file "file.txt" on the terminal using the less command, which allows for scrolling through the file. The > operator is used to redirect the output of the cat command to a new file, and the | operator is used to pipe the output of one command to another command.


### echo
`echo` is a command used in Unix-like operating systems to print text to the terminal or redirect it to a file. It allows users to output text or variables as text strings. The basic syntax of the `echo` command is `echo [option] [string]`. The `[option]` parameter is optional and can be used to modify the behavior of the `echo` command, while the `[string]` parameter is the text that you want to print or redirect.

1. To display a message on the terminal:
    ``` bash
    echo "Hello, World!"
    ```
    > Note: This will print the message "Hello, World!" on the terminal.

2. To redirect text to a file:
    ``` bash
    echo "This is a text file." > text.txt
    ```
    > Note: This will create a new file named "text.txt" and write the text "This is a text file." to it.

3. To append text to an existing file:
    ``` bash
    echo "This is more text." >> text.txt
    ```
    > Note: This will append the text "This is more text." to the end of the existing "text.txt" file.

4. To use a variable in an echo statement:
    ``` bash
    NAME="John"
    echo "My name is $NAME."
    ```
    > Note: This will print the message "My name is John." on the terminal, using the variable $NAME in the text string. The > operator is used to redirect the output of the echo command to a new file, and the >> operator is used to append the output to an existing file.


### >
The `>` operator is used in Unix-like operating systems to redirect the output of a command to a file. It allows users to create a new file or overwrite the contents of an existing file with the output of a command. The basic syntax of the `>` operator is `command > file`. The `command` parameter represents the command whose output you want to redirect, and the `file` parameter represents the file that you want to redirect the output to.

1. To redirect the output of a command to a file instead of displaying it on the terminal:
    ``` bash
    ls -la > file_list.txt
    ```
    > Note: This will run the ls command with the -la option, which lists all files in the current directory, including hidden files, and redirects the output to a new file named "file_list.txt".

### >>
The `>>` operator is used in Unix-like operating systems to append the output of a command to an existing file. It allows users to add new content to the end of a file without overwriting any existing content. The basic syntax of the `>>` operator is `command >> file`. The `command` parameter represents the command whose output you want to append, and the `file` parameter represents the file that you want to append the output to.


1. To append the output of a command to an existing file:
   ``` bash
   ls -la >> file_list.txt
   ```
   > Note: This will run the ls command with the -la option, which lists all files in the current directory, including hidden files, and append the output to an existing file named "file_list.txt".




### |
The `|` (pipe) operator in Unix-like operating systems is used to redirect the output of one command to the input of another command. It allows users to chain together multiple commands to perform more complex operations without having to save intermediate results to files. The basic syntax of the `|` operator is `command1 | command2`. The `command1` parameter represents the command whose output you want to redirect, and the `command2` parameter represents the command that will receive the redirected output as input.

1. To list all files in the current directory and then search for a specific file within that list:
    ``` bash
    ls | grep specific_file
    ```
    > Note: This will list all files in the current directory and then search for the string "specific_file" within that list.

2. To count the number of files in the current directory:
    ``` bash
    ls | wc -l
    ```
    > Note: This will list all files in the current directory and then count the number of lines in the output, which is equivalent to the number of files in the directory.

3. To sort the output of a command alphabetically:
    ``` bash
    command | sort
    ```
    > Note: This will run the command and sort the output alphabetically. The | operator can be used with any command that produces output to the console. It is a powerful tool for chaining together commands to perform more complex operations.


### rm
The `rm` command in Unix-like operating systems is used to remove or delete files and directories. The basic syntax of the `rm` command is `rm [options] [file(s)]`. The `options` parameter represents any additional options you want to use with the command, and the `file(s)` parameter represents the name(s) of the file(s) you want to remove. By default, `rm` does not prompt for confirmation before deleting files, so it's important to be careful when using this command.

1. To remove a single file:
    ``` bash
    rm filename.txt
    ```
    > Note: This will remove the file named "filename.txt" from the current directory.

2. To remove multiple files at once:
    ``` bash
    rm file1.txt file2.txt file3.txt
    ```
    > Note: This will remove the files named "file1.txt", "file2.txt", and "file3.txt" from the current directory.

3. To remove a directory and all its contents:
    ``` bash
    rm -r directory_name
    ```
    > Note: This will remove the directory named "directory_name" and all its contents, including any files and subdirectories. The -r option is required to remove directories with rm, as directories are not removable by default. It's important to be careful when using the rm command, as it permanently deletes files and directories without any way to recover them.



### curl
`curl` is a tool used to transfer data to or from a server, using one of several supported protocols, including HTTP, FTP, and SMTP. The basic syntax of the `curl` command is `curl [options] [URL]`. The `options` parameter represents any additional options you want to use with the command, and the `URL` parameter represents the URL of the server you want to communicate with.

1. To retrieve the contents of a web page:
    ``` bash
    curl https://example.com
    ```
    > Note: This will retrieve the contents of the web page at https://example.com and display it in the terminal.

2. To download a file from a server:
    ``` bash
    curl -O https://example.com/file.txt
    ```
    > Note: This will download the file named file.txt from the server at https://example.com and save it to the current directory.

3. To upload a file to a server:
    ``` bash
    curl -F "file=@/path/to/file.txt" https://example.com/upload.php
    ```
    > Note: This will upload the file located at /path/to/file.txt to the server at https://example.com/upload.php using a POST request.



### wget
`wget` is a tool used to download files from the internet. It supports various protocols such as HTTP, HTTPS, and FTP. Its basic syntax is `wget [options] [URL]`. The `options` parameter represents any additional options you want to use with the command, and the `URL` parameter represents the URL of the file you want to download. `wget` is a powerful tool that can be used to download large files, recursively download entire directories, and continue interrupted downloads.

1. Download a file from a URL:
    ``` bash
    wget https://example.com/file.zip
    ```

2. Download a file and save it with a different name:
    ``` bash
    wget -O newfile.zip https://example.com/file.zip
    ```
    
3. Download a file and continue the download if it is interrupted:
    ``` bash
    wget -c https://example.com/largefile.iso
    ```

4. Download multiple files from a URL:
    ``` bash
    wget -i urls.txt
    ```
    > Note: where urls.txt is a text file containing one URL per line.



5. Limit the download speed:
    ``` bash
    wget --limit-rate=500k https://example.com/largefile.iso
    ```

6. Download a file over FTP:
    ``` bash
    wget ftp://ftp.example.com/file.zip
    ```

7. Download a file using a proxy server:
    ``` bash
    wget --proxy=on --proxy-user=user --proxy-password=pass https://example.com/file.zip
    ```







### screen
`screen` is a terminal multiplexer that allows you to create and manage multiple terminal sessions within a single window. With `screen`, you can run multiple shell instances, detach from them and reattach to them later, and share sessions with other users. Once inside a screen session, you can use various keyboard shortcuts to navigate between multiple windows, split screens, and perform other tasks. `screen` is particularly useful for remote server management or for running long-running processes that you want to keep running even if you log out of your shell.

1. Start a new screen session with a specific name:
    ``` bash
    screen -S mysession
    ```

2. Detach from a screen session:
    ``` text
    Press `Ctrl-a` followed by the `d` key.
    ```

3. Reattach to a detached screen session:
    ``` bash
    screen -r mysession
    ```
    
4. Create a new window within a screen session:
    ``` text
    Press `Ctrl-a` followed by the `c` key.
    ```

5. Switch between windows in a screen session:
    ``` text
    Press `Ctrl-a` followed by the `n` key to move to the next window
    or `Ctrl-a` followed by the `p` key to move to the previous window.
    ```
    
6. Split the screen horizontally:
    ``` text
    Press `Ctrl-a` followed by the `S` key.
    ```

7. Split the screen vertically:
    ``` text
    Press `Ctrl-a` followed by the `|` key.
    ```

8. List available screen sessions:
    ``` bash
    screen -ls
    ```


### tar
The `tar` command is used for archiving and compressing files in a single file, often called a "tarball". It is a command-line utility commonly used in Linux and Unix operating systems.

1. To create a compressed tarball of a directory and its contents:
    ``` bash
    tar -czvf myfiles.tar.gz /path/to/my/directory/
    ```

2. To extract a compressed tarball to a specific directory:
    ``` bash
    tar -xzvf myfiles.tar.gz -C /path/to/extracted/directory/
    ```

3. To add a file to an existing tarball:
    ``` bash
    tar -rvf myfiles.tar /path/to/newfile.txt
    ```

4. To extract a specific file from an existing tarball:
    ``` bash
    tar -xvf myfiles.tar /path/to/file.txt
    ```

5. To create an incremental backup of a directory using a dated tarball filename:
    ``` bash
    tar -czvf myfiles-$(date +%Y%m%d).tar.gz --listed-incremental=/path/to/backup.snar /path/to/my/directory/
    ```


### unzip
The `unzip` command is used to extract files from a compressed archive in the ZIP format. Here's a short explanation:

1. To extract all files from an archive named archive.zip:
    ``` bash
    unzip archive.zip
    ```

2. To extract a specific file named example.txt from an archive named archive.zip:
    ``` bash
    unzip archive.zip example.txt
    ```

3. To extract an archive named archive.zip into a directory named extracted_files:
    ``` bash
    unzip archive.zip -d extracted_files/
    ```

4. To list the contents of an archive named archive.zip without extracting them:
    ``` bash
    unzip -l archive.zip
    ```


### dtrx
The `dtrx` command is a tool used for extracting various archive file formats. It can automatically detect the archive type and use the appropriate extraction tool. It can also handle nested archives, and can extract files to a specific directory.

1. To extract a single archive file named `archive.tar.gz` to the current directory:
    ``` bash
    dtrx archive.tar.gz
    ```

2. To extract a nested archive file named `nested_archive.zip` that is located within another archive file named `archive.tar.gz` to the current directory:
    ``` bash
    dtrx archive.tar.gz
    cd archive
    dtrx nested_archive.zip
    ```

3. To extract a single archive file named `archive.tar.bz2` to a specific directory named `my_folder`:
    ``` bash
    dtrx -n my_folder archive.tar.bz2
    ```

4. To list the contents of an archive file named archive.tar.gz without extracting them:
    ``` bash
    dtrx -l archive.tar.gz
    ```

## Create and manage permissions, security, and services

### chmod

### chown

### whoami

### adduser

### usermod

### su

### ssh

### ssh-keygen

### ufw

### systemctl

## Some helpful commands

### sudo

### !!

### top

### ps

### grep

### netstat

### ifconfig

### iptables

### df

### openssl

### rsync



