tmux Cheatsheet
===============

General
-------

Concept hierarchy

    Session > Window > Pane

Configured leader prefix: `M-a`. In config file `~/.tmux.conf`

    set-option -g prefix M-a

To reload configuration

    $ tmux source-file ~/.tmux.conf

Sessions
--------

Create a new session and attach

    $ tmux

Detach from current session

    (pref) d

Attach to existing session

    $ tmux attach [-t 3]

List sessions

    $ tmux list-sessions

Kill session

    $ tmux kill-session [-t 3]
    Ctrl-d

Windows
-------

Create new window

    (pref) c

Go to specific window

    (pref) 3

Go to next window

    (pref) n

Go to previous window

    (pref) p

Move current window to number 2

    $ tmux movew -t2

Move window 2 to number 1

    $ tmux movew -s2 -t1

Panes
-----

Split horizontally

    $ tmux split-window -h
    (pref) %

Split vertically

    $ tmux split-winsow -v
    (pref) "

Go to panel...

    (pref) LEFT | RIGHT | UP | DOWN

Zoom in/out a panel

    (pref) z

Clipboard
---------

TODO
