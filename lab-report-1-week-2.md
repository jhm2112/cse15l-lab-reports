
# Lab Report 1 <br />
## Logging into an ieng6  account <br />
<br />



**Downloading and installing VSCode** <br />
<br />
The first step is to download and install VSCode. Go to https://code.visualstudio.com/download and choose the version that is compatible with your machine. Then follow the instructions to install.

![Image](vscode.png) <br />


**Remotely Connecting** <br />
<br />
*First step for Windows users only: install a program called OpenSSH.* <br />
 <br />
1. After installing VSCode, go to https://sdacs.ucsd.edu/~icc/index.php and look up your CSE15L course-specific account.

2. Open a terminal in VSCode and input this command (with the *zz* replaced by the letters in your account) :

   `$ ssh cs15lwi22zz@ieng6.ucsd.edu`
3. Type yes to the prompt that follows and input your password to log in 

4. Once you are logged in, you should see something like this:

![Image](terminal1.png) <br />
<br />

**Sample commands** <br />

Now that you are logged in, you can try running some commands. Here are some for you to try:

* **cd**: change directory to the home directory
* **ls**: lists the files in the current directory
* **ls -a**: lists ALL files in the current directory (files starting with ".")
* **mkdir <name_of_directory>**: creates a directory
* **pwd**:  prints the path of the current directory
* **cp <Source_file> <Destination_file>**: copies the contents of source file into destination file.

For example, running the `ls -a` and `ls` commands:

![Image](ls.png)
>Note that `ls` lists less files than `ls -a `

<br />


**Moving Files with `scp`**

To copy a file from your machine to the server, we will use this command:

`scp FileName.extension cs15lwi22zz@ieng6.ucsd.edu:~/`

Replacing *FileName.extension* with the desired file name and *zz* with your account's specific letters. You will need to enter your password after entering the command.

For example, we will copy *sampleTutorial.txt*:

![Image](beforeCopy.png)
>Listing the files before copying *sampleTutorial.txt*

<br />

![Image](copyCommand.png)
>This is how the command looks in this particular example

<br />

![Image](afterCopy.png)
>After copying. We can see that *sampleTutorial.txt* is now listed

<br />
<br />

**Setting an SSH Key**

















	