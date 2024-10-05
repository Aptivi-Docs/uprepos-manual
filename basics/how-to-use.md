---
description: How do you use this script?
icon: question
---

# How to use?

Running this script is so easy, especially when you have to check hundreds of repositories in your Git repository library (a directory containing your Git repositories) for updates on the remote side.

To check for updates on the current Git repository library, just run the script with no arguments:

```
$ uprepos
```

To check for updates on any specified directory, run the script with the relative or absolute path to the directory containing your repositories:

```
$ uprepos Path/To/Repos
```

Internally, it will call the following commands:

```
$ git -C Path/To/Repos fetch
$ git -C Path/To/Repos pull --recurse-submodule
$ git -C Path/To/Repos submodule update --remote
```

{% hint style="info" %}
Depending on the repository size and your network connection speed, it might take a while.
{% endhint %}
