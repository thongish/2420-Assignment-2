# 2420-Assignment-2

# Table of contents
- [Introduction](#introduction)
- [Project 1](#project-1)
- [Project 2](#project-2)

# Introduction
This is my assignment 2 repository which holds 2 separate bash scripting projects.

To get started using these scripts, ensure you have git installed on your system and clone the repository:
```
git clone https://github.com/thongish/2420-Assignment-2.git
```

After that, change directory into `project-1` or `project-2`, depending on which script you want to use.

## Project 1:
A set of scripts that automate the setup of a new Linux Distro installation by installing packages and setting up configuration files. 

It is comprised of 4 different files:
- `configsetup` - This is a script that clones an example dotfile repository from https://gitlab.com/cit2420/2420-as2-starting-files and creates the necessary directories and symbolic links.
- `packagesetup` - This is a script that installs packages on Arch Linux systems using a user-defined list of packages in the `package-list` file.
- `package`-list - This is a plain text file where you can define what packages you want the scripts to install.
- `setup` - This is a script that can run either the configsetup or packagesetup scripts or both using options.

### Usage:
```
sudo ./setup <option(s)> <username>
```

Available options:
- `-i` - Run the `packagesetup` script.
- `-c` - Run the `configsetup` script.

### Examples:
```
sudo ./setup -i my_user
sudo ./setup -c my_user
sudo ./setup -ic my_user
```
