# RaspberryPi4
Adventures with my Raspberry Time 4b 

# Navigation
*  [Visual Studio Code](VsCode.md) - *For Raspberry Pi*
*  [Clang & LLVM](ClangAndLLVM.md) - *Code*
*  [SDL2](SDL2.md) - *Install and build SDL2 libraries*

# Quick Instructions 

## SSH Key

```bash
# Go to the ssh folder
$ cd ~/.ssh

# Generate ssh key files and replace <email> with your own email address
$ ssh-keygen -t rsa -b 4096 -C "<email>"
```

You will be asked to give the file a name but the default name will be chosen if you just press enter.

It will also ask you for a password and you will have to choose if you want to write it every time you use a SSH connection with these key pairs or not. It might make sense with no password for something on your local network but a password is reccomended for external services.

### Start SSH Agent

```bash
$ eval $(ssh-agent -s)
```

### Add key to agent

```bash
$ ssh-add ~/.ssh/id_rsa
```

### Add GitHub or other service

It is the public half of your key that you should only share.

```bash
# Display the public key in the terminal
$ cat ~/.ssh/id_rsa.pub
```

Select the complete key, mail address and all.

Then press CTRL + SHIFT + C to copy it.

#### Github

Go to [GitHub SSH Keys Management](https://github.com/settings/keys) and add the key.

It is a good idea to give the key a proper name for the future ;)
