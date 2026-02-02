---
description: Welcome to uprepos!
icon: hand-wave
---

# Welcome!

Welcome to `uprepos`, which is a very small `bash` script that lets you update all your repositories found under a folder containing all your Git repositories.

It's an abstraction of a set of commands that you'll have to execute to update all repositories in a folder so that you can save your time from having to manually update them. `uprepos` attempts to execute the following commands for every directory:

```shellsession
$ git -C Path/To/Repos fetch
$ git -C Path/To/Repos pull --recurse-submodule
$ git -C Path/To/Repos submodule update --remote
```

Remembering and writing all those commands manually is time-consuming, especially if you need a quick shortcut to all the above commands.
