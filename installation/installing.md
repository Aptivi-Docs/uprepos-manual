---
description: How to install this script.
icon: compact-disc
---

# Installing

Installing this script is easy. To install it, follow these steps, assuming that you have either `CURL` or `wget` installed on your Linux system:

## Local and System-wide

There are two ways to install this script on your system. If you want to make this script available to all the users on your Linux system, be sure to install it on your home directory like this:

```
$ curl -fsSL https://raw.githubusercontent.com/Aptivi/uprepos/main/uprepos > $HOME/uprepos
$ chmod +x $HOME/uprepos
```

If you want to make this script available to all of the users installed, follow these two scripts as root (`sudo`):

```
$ curl -fsSL https://raw.githubusercontent.com/Aptivi/uprepos/main/uprepos | sudo tee /usr/local/bin/uprepos
$ sudo chmod +x /usr/local/bin/uprepos
```

If you prefer using wget to install the script, follow these steps:

* For local installs

```
$ wget -O$HOME/uprepos https://raw.githubusercontent.com/Aptivi/uprepos/main/uprepos
$ chmod +x $HOME/uprepos
```

* For system-wide installs

```
$ sudo wget -O/usr/local/bin/uprepos https://raw.githubusercontent.com/Aptivi/uprepos/main/uprepos
$ sudo chmod +x /usr/local/bin/uprepos
```

{% hint style="info" %}
For MinGW, WSL, and Git Bash installs, only the local install is supported.
{% endhint %}
