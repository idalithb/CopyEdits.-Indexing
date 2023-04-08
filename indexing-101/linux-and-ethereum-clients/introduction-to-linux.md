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
`cp` is a command used in Unix-like operating systems to copy files or directories. It allows users to create a duplicate copy of an existing file or directory. The basic syntax of the cp command is cp source destination. The source parameter is the file or directory that you want to copy, and the destination parameter is where you want to copy the file or directory to.

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
`mv`

### cat
`cat`

### echo
`echo`

### >
`>`

### |
`|`

### rm
`rm`

### curl
`curl`

### wget
`wget`

### tar
`tar`

### unzip
`unzip`

### dtrx
`dtrx`

