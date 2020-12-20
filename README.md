# Tony's personal Debian package repository

## Introduction
The repository is used to collect some Debian packages whinch are not in the official repo.

## Usage
Add the public GPG key to the apt sources keyring.
```
wget -qO - https://blog.iamsjy.com/packages/PUBLIC.KEY  | sudo apt-key add -
```

Edit `/etc/apt/sources.list`
```
sudo nano /etc/apt/sources.list
```
Then, add the following line.
```
deb https://blog.iamsjy.com/packages buster main
```
Save this file, then refresh the apt configuration.
```
sudo apt update
```
Now you can use `sudo apt install PACKAGE_NAME` to install packages from the repo.
