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
`touch`

### git
`git`

### nano
`nano`

### vim
`vim`

### cp
`cp`

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

