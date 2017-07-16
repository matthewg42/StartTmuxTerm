StartTmuxTerm
=============

This software makes it convenient to run a terminal which starts in one of several pre-defined tmux sessions. Upon invokation, the program opens a menu centered on the screen with a list of session types. Clicking a session opens a terminal for that session.

If a session of that type is already running, the new terminal window will attach to it, else a new session will be created.

Shift-clicking on a session name stars that session, and also sets it to be the default session type.

The cursor keys can also be used to select a session.  RETURN starts the selected session, Shift+RETURN also selects it as the default session for future invokations.  

Pre-requisites
--------------

* Python3
* PyQt5

Setup
-----

* Copy the tmux directory to your home directory, renaming it to .tmux, and
* Copy bin/StartTmuxTerm to a bin directory and make it executable, i.e.

```shell
$ cp -Rp tmux ~/.tmux
$ sudo install -m 755 bin/StartTmuxTerm /usr/local/bin
```

To Do
-----

* Support multiple terminal emulators with good default settings for each

