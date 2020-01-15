st - simple terminal, slightly modified
=======================================
The simple terminal, [st](https://st.suckless.org/), is another [suckless](https://suckless.org/) creation meant to deliver a terminal emulator with as little bloat as possible.

Key bindings
------------
st, like most software from suckless, is driven from the keyboard. Things like scrollbars are not deemed useful enough to be implemented since you can just as easily scroll using the keyboard. 
* `Alt+K/J` or `Alt+Up/Down` scrolls up/down; pressing `Ctrl+Shift` instead of `Alt` (ex. `Ctrl+Shift+K`) jumps 25 lines instead of just 1
* `Alt+C/V` is bound to copy/paste
* `Ctrl+Shift+Enter` opens a new terminal in your current directory
* `Ctrl+Shift+L/H`, `Ctrl+Shift+Right/Left` or `Ctrl+Shift+PageUp/PageDown` to increse/decrease font size; `Ctrl+Shift+0` or `Ctrl+Shift+Home` resets to default

Original README
===============
st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

