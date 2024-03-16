# Web3-DApps
Learning Web3-Decentralised Apps(DApps) Development
## Installation and Setup for Windows

#### for Internet Computer Web3 Application Development
<br>
https://docs.google.com/document/d/e/2PACX-1vTNicu-xuf4EiLAehHIqgfpjAnPjzqMGT-xpZVvYaAWNyvzYK_Ceve_me4PVRIxpzH7ea5PAX9NxGwY/pub

## Requirements
Windows 10 or higher (version 2004 or higher). Build 19041.xxx or higher.
64-bit machine (System type x64 based PC)
Example: search System information and check requirments 
![req1](https://github.com/DEvackemann/Web3-DApps/assets/150266045/6839a4a9-a8ce-486b-8f86-99f9db3b8068)
### Steps
#### WSL(Window powerShell)
1.Find the Windows PowerShell in your Start menu and run it as the Administrator.

2.WSL is the Windows Subsystem for Linux and it will allow us to run command line commands in Windows. Here’s more info from Microsoft: ​​
https://docs.microsoft.com/en-us/windows/wsl/install

3.As described in the docs above, we need to paste this command into PowerShell and hit enter:

```
wsl --install
```
4.Once that’s done, you’ll need to restart your computer.

5.Upon restart you will be prompted to setup an ubuntu username and password and then you will have successfully installed WSL. (Keep a note of both of these pieces of information, you’ll need it later on).
Note: when you type your password it will not show up, just make sure you know what you’re typing! Remember your password it required in further steps!!

6.To confirm that everything worked correctly, type the following command into PowerShell:
```

wsl --list --verbose
```
7.You should see it output something like this:
![req2](https://github.com/DEvackemann/Web3-DApps/assets/150266045/e8168fad-ec9b-4d45-922d-fbe1a0c8090d)


## VSCode
8.  Download and install the latest version of VSCode from here:

https://code.visualstudio.com/


9.  Install the Motoko language extension in VSCode (make sure it’s from the Dfinity team, or just use the link below).

https://marketplace.visualstudio.com/items?itemName=dfinity-foundation.vscode-motoko


10.  Install the Remote WSL extension.

https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl

## Node
11. Search and open up Ubuntu from the Start menu.


12.  Type the following command to install homebrew (Alternatively copy it from the homebrew website https://brew.sh/):
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
Homebrew will make it easier for us to install other tools such as node. You might already have node installed on your windows system but because we’re working with WSL, you’ll need to install it on the linux system too.


13. goto ubunto When prompted enter the password for the user that you set previously in step 5.
![req3](https://github.com/DEvackemann/Web3-DApps/assets/150266045/5409affc-c008-41b7-b5e7-cedffc8fa03d)


14 .  The installer will tell you how to add brew to the PATH. Copy the  commands they list and run them one by one in Ubuntu.
check Next steps and copy the path

e.g.![req4](https://github.com/DEvackemann/Web3-DApps/assets/150266045/d128c20c-9714-4d17-b9c2-16262390a481)

15. Also run the command under the line “Install Homebrew’s dependencies if you have sudo access”:
```
sudo apt-get install build-essential
```

16. Check that everything worked by typing the command:
```
brew --version
```
If you see a version show up then everything was installed.


17. Install node using homebrew with the following command:
```
brew install node@16
```

18. Once it’s done check that it worked with:
```
node --version
```
NOTE:If you got error {node@16 is key only ,which means its not syntax into path.. } or If you have another version of node installed (e.g. previous version or windows version) then you need will to link the version we just installed to homebrew use the command: 
![req5](https://github.com/DEvackemann/Web3-DApps/assets/150266045/924c417b-aab3-4244-9b8e-2e44b51c16be)

```
brew link node@16
```





