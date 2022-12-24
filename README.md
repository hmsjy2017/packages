# Tony's personal Debian package repository

## Introduction
The repository is used to collect some Debian packages whinch are not in the official repo.

## Usage
Add the public GPG key to the apt sources keyring.
```
wget -qO - https://hmsjy2017.github.io/packages/public.key  | sudo apt-key add -
```

Edit `/etc/apt/sources.list`
```
sudo nano /etc/apt/sources.list
```
Then, add the following line.
```
deb https://hmsjy2017.github.io/packages buster main
```
Save this file, then refresh the apt configuration.
```
sudo apt update
```
Now you can use `sudo apt install PACKAGE_NAME` to install packages from the repo.

(Replace `PACKAGE_NAME` with the name of the package you want to install)

If the speed is too slow, you can try the [mirror addresses](#mirrors).

## Mirrors

* Netlify
```
https://debian-packages.netlify.app/
```
* Vercel
```
https://apt.vercel.app/
```
