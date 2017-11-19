---
layout: default
title: .screenrc
---

```bash
##############################################################################
# modifications
##############################################################################

# selects panes with mouse
mousetrack on

##############################################################################
# remappings
##############################################################################

# Ctrl-j = Ctrl-a
escape ^Jj

# V = vertical split and automatically switches to it
bind 'V' eval "split -v" focus screen

# S = split and automatically switches to it
bind 'S' eval split focus screen

# e = resizes windows to be equal
bind 'e' resize =

# resizes windows
bind '+' resize +5
bind '-' resize -5

```

---

## Default key bindings

```
DEFAULT KEY BINDINGS
As  mentioned,  each  screen  command  consists of a "C-a" followed by one other character.  For your conve‐
nience, all commands that are bound to lower-case letters are also bound to their control character counter‐
parts (with the exception of "C-a a"; see below), thus, "C-a c" as well as "C-a C-c" can be used to create a
window. See section "CUSTOMIZATION" for a description of the command.

The following table shows the default key bindings:
C-a '       (select)      Prompt for a window name or number to switch to.
C-a "       (windowlist -b)
                          Present a list of all windows for selection.
C-a 0       (select 0)
 ...           ...
C-a 9       (select 9)
C-a -       (select -)    Switch to window number 0 - 9, or to the blank window.
C-a tab     (focus)       Switch the input focus to the next region.  See also split, remove, only.
C-a C-a     (other)       Toggle to the window displayed previously.  Note that this binding defaults to the
                          command  character  typed  twice, unless overridden.  For instance, if you use the
                          option "-e]x", this command becomes "]]".
C-a a       (meta)        Send the command character (C-a) to window. See escape command.
C-a A       (title)       Allow the user to enter a name for the current window.
C-a b
C-a C-b     (break)       Send a break to window.
C-a B       (pow_break)   Reopen the terminal line and send a break.
C-a c
C-a C-c     (screen)      Create a new window with a shell and switch to that window.
C-a C       (clear)       Clear the screen.
C-a d
C-a C-d     (detach)      Detach screen from this terminal.
C-a D D     (pow_detach)  Detach and logout.
C-a f
C-a C-f     (flow)        Toggle flow on, off or auto.
C-a F       (fit)         Resize the window to the current region size.
C-a C-g     (vbell)       Toggles screen's visual bell mode.
C-a h       (hardcopy)    Write a hardcopy of the current window to the file "hardcopy.n".
C-a H       (log)         Begins/ends logging of the current window to the file "screenlog.n".
C-a i
C-a C-i     (info)        Show info about this window.
C-a k
C-a C-k     (kill)        Destroy current window.
C-a l
C-a C-l     (redisplay)   Fully refresh current window.
C-a L       (login)       Toggle this windows login slot. Available only if screen is configured to update the utmp database.
C-a m
C-a C-m     (lastmsg)     Repeat the last message displayed in the message line.
C-a M       (monitor)     Toggles monitoring of the current window.
C-a space
C-a n
C-a C-n     (next)        Switch to the next window.
C-a N       (number)      Show the number (and title) of the current window.
C-a backspace
C-a h
C-a p
C-a C-p     (prev)        Switch to the previous window (opposite of C-a n).
C-a q
C-a C-q     (xon)         Send a control-q to the current window.
C-a Q       (only)        Delete all regions but the current one.  See also split, remove, focus.
C-a r
C-a C-r     (wrap)        Toggle the current window's line-wrap setting (turn the current window's automatic margins on and off).
C-a s
C-a C-s     (xoff)        Send a control-s to the current window.
C-a S       (split)       Split the current region horizontally into two new ones.  See also only, remove, focus.
C-a t
C-a C-t     (time)        Show system information.
C-a v       (version)     Display the version and compilation date.
C-a C-v     (digraph)     Enter digraph.
C-a w
C-a C-w     (windows)     Show a list of window.
C-a W       (width)       Toggle 80/132 columns.
C-a x
C-a C-x     (lockscreen)  Lock this terminal.
C-a X       (remove)      Kill the current region.  See also split, only, focus.
C-a z
C-a C-z     (suspend)     Suspend screen.  Your system must support BSD-style job-control.
C-a Z       (reset)       Reset the virtual terminal to its "power-on" values.
C-a .       (dumptermcap) Write out a ".termcap" file.
C-a ?       (help)        Show key bindings.
C-a C-\     (quit)        Kill all windows and terminate screen.
C-a :       (colon)       Enter command line mode.
C-a [
C-a C-[
C-a esc     (copy)        Enter copy/scrollback mode.
C-a C-]
C-a ]       (paste .)     Write the contents of the paste buffer to the stdin queue of the current window.
C-a {
C-a }       (history)     Copy and paste a previous (command) line.
C-a >       (writebuf)    Write paste buffer to a file.
C-a <       (readbuf)     Reads the screen-exchange file into the paste buffer.
C-a =       (removebuf)   Removes the file used by C-a < and C-a >.
C-a ,       (license)     Shows where screen comes from, where it went to and why you can use it.
C-a _       (silence)     Start/stop monitoring the current window for inactivity.
C-a |       (split -v)    Split the current region vertically into two new ones.
C-a *       (displays)    Show a listing of all currently attached displays.
```