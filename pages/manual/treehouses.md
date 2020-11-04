#Treehouses

## Objectives

* Getting familiar with treehouses cli 
* Set up your SSH key
* Set up Tor

### Treehouses cli

Treehouses cli is already included in Planet Vagrant. So after you login to vagrant of planet system you can run treehouses commands. Treehouses cli command starts with `treehouses` keyword.
There are lot of subcommands for treehouses which you can look into by running
`treehouses help` on your terminal.
You can explore and try out different commands on your own, but we will focus here only few commands.

### Create your SSH key

Follow these steps to create your SSH key:
- [Generate a new SSH key and add it to the ssh-agent](https://help.github.com/en/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)  
- [Add the SSH key to your GitHub account](https://help.github.com/en/articles/adding-a-new-ssh-key-to-your-github-account)

**NOTE**: With `cat ~/.ssh/id_rsa*` you can check your SSH key pair. Both parts (private and public) of your recently created SSH key should show up. Please be sure that your (private) key is protected by a passphrase and has been created on your computer.

A trick to whether github is configured correctly is to navigate to `https://github.com/<yourgithubusername>.keys` in a browser - your public SSH key should show up there.

**NOTE**: Be sure not to confuse the public SSH key and the key fingerprint. The fingerprint of a key is unique and used to identify the key. 

SSH keys are stored in a `~/.ssh` directory. You will need to find a set of files looking like `id_dsa` or `id_rsa` (your private key or key fingerprint) and a complimentary `.pub` file (your public key).
This is the key fingerprint format: `SHA256:PqNGgIJfgjnoq9JMd2czLPAevkAzr4OIKb22GxMZg1M dogi@ole.org`.
However, the public keys are similar to this: 
```
$ cat ~/.ssh/id_rsa.pub
ssh-rsa AAAAB3NzaC1yc2EAAAABIwAAAQEArMkyotKz1J5+Kux3ToBNe+X3Qm+6WzTXflEEeOWdmxDZ5f5le7Ujes81ybRnavWSNR2TGr1evigE7vGsxHm2aEeR0YICWR24lPcJ2FUROmEdwn2OjDzh1YcKJDNvlMzXt1x0dNeEkSisHpk6p5RJ7OfCtyD/OjKhGyajbxS/n3RDSMgND46M7AiiaaIzlut3D09Gyhd93t16NTyR9Ej1RRRk8z9of3qLwhC1AqVJpSkuWn9+q111AfljsVZCHHDLw0+j7NIntk5x+yzrl2QQECNEaPpm1Pt4gmLG2nnrNjPAtrjWIfyWfhdSbgk/QscAE2XpCYoSFBW9d8bdIVMfSw== dogi@ole.org
```

## Tor
Tor is a computer network run by volunteers worldwide. Each volunteer runs what is called a relay, which is just a computer that runs software allowing users to connect to the Internet via the Tor network.

Before hitting the open Internet, the Tor Browser will connect to several different relays, wiping its tracks each step of the way, making it difficult to figure out where, and who, you really are.

The Systems Team utilizes this tool to provide a further layer of security when interacting with the Machines deployed in the field.

Please start by watching this [video](https://www.youtube.com/watch?v=6czcc1gZ7Ak) about the Tor browser.

### Get Tor

#### macOS

You should already have [Homebrew](https://brew.sh) installed.  You can check if it's already installed by running `brew -v` in your terminal.  If you haven't yet installed it, run the following:
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew install wget cask
```

Then, install Tor and Tor Browser:
```
brew install tor
brew cask install tor-browser
```

#### Windows & Linux

Install [Tor](https://www.torproject.org/download/)


### Turn on Tor

To activate Tor, SSH into your Vagrant. You might need to access it as `root` by executing `sudo -s`. Then run `treehouses tor add 22`, `treehouses tor add 80`, `treehouses tor add 2200` and `treehouses tor notice on`.  To view the Tor address of your machine, run `treehouses tor`, then copy and paste this address into your Tor Browser, to make sure it works; you should see a configuration page for Planet Learning, one of our other services.

---
#### At the end of this section, post the code of your successful SSH terminal with tor address to the [Slack chat](http://slack.ole.org)

It may look like this:
```
vagrant ssh

Linux prod 4.19.0-9-amd64 #1 SMP Debian 4.19.118-2 (2020-04-29) x86_64


The programs included with the Debian GNU/Linux system are free software;                                                                                                                                                         
the exact distribution terms for each program are described in the                                                                                                                                                                
individual files in /usr/share/doc/*/copyright.                                                                                                                                                                                   

Debian GNU/Linux comes with ABSOLUTELY NO WARRANTY, to the extent
permitted by applicable law.
Last login: Thu Aug 22 23:20:37 2019 from unknown.comcast.net
vagrant@prod:~#
```

---

You can find instructions on Code and Syntax Highlighting [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#code-and-syntax-highlighting)
