<h2>Installing VScode</h2>
To install VSCode, go to [the VSCode Website](https://code.visualstudio.com/) . Click on the big blue button to download and run the installer to install.
![](OPENSSH%20CLIENT%20AND%20SERVER.png)

<h2>Remotely Connecting</h2>
To connect to the lab computers remotely, make sure that open ssh is installed on your windows device by going to settings > searching for "optional features" > checking from the dropdown list that both the "OpenSSH Client" and "OpenSSH Server" are installed.
Then, in VSCode, open a new terminal (by pressing "ctrl" + "~") and type in "ssh cs15lfa22**@ieng6.ucsd.edu" where the two asterisks are replaced with the two characters associated with your CSE 15L account (can be found at [this site](https://sdacs.ucsd.edu/~icc/index.php))
You should be able to enter in your account password. I (and many other of my peers) had trouble with this.
![](VSCODE%20WEBSITE.png)
![](SSHTERMINAL.png)
![](SUCCESSFULLOGIN.png)

<h2>Trying Some Commands</h2>
Despite not being able to be remotely connected to the lab computers, I can still show you how to use some of the commands you will use! 
"cd" indicates that you will be updating the directory you are working in, adding more file paths after it moves you around your filesystem. Putting a tilde after it returns you to the home directory.
ls denotes linux commands. -lat displays a lot of files in the directory laterally, and -a displays all of them
cp is our way to compile files on the remote computers, and cat is our way to run them

![](TERMINAL%20COMMANDS.png)
![](BUNCHOFCOMMANDS.png)

<h2>Moving Files with scp</h2>
we're able to create, compile, and run a java file within vscode
![](RUNJAVA.png)
however, I cannot show you any of the sending of the files to the remote computer because my secure copy (scp) does not work because I am not able to connect to the computers with ssh.

<h2>Setting an SSH Key</h2>
We would next generate a set of public and private keys and sent the files with them over to the remote computer so that we would not have to enter passwords in each time we logged in. I cannot show you the process of sending it over nor the process of logging in smoother (or at all), but I can show how to generate the keys. Just type in "ssh-keygen -t ed25519". It will ask you to enter a file location to save the keys, but pressing enter to use the default works fine. It will then ask for passwords, but setting no password also works fine here. After that, it will visualize everything it has generated, and you can see the files for the keys at the file folder you chose.
![](KEYGEN.png)

<h2>OPTIMIZATIONS</h2>
The only thing left to show is optimizations. I can't show any related to logging in, but I can show how you can run multiple commands from the command line with a semicolon!

![](OPTIMIZATIONSWOO.png)
