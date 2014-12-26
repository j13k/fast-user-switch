# Fast User Switch workflow

_Fast User Switch_ is a Mac OS X Automator workflow that can be assigned to a system-wide hotkey for _really_ fast user switching.

It has been adapted from a workflow described in a CNET article, [How to create a hot key to switch users in OS X](http://www.cnet.com/news/how-to-create-a-hot-key-to-switch-users-in-os-x/), and tweaked to enable switching to users not yet logged in.

## Installation instructions 

1. Clone the repository, or [download](https://github.com/j13k/fast-user-switch/releases/latest) and unpack an archive.
1. Open the _Fast User Switch.workflow_ package and select the option to install it as a service. (Feel free to open the workflow in Automator first to check out what it does—this is probably a good idea with any third-party workflows.) 
1. Open the Keyboard pane in System Preferences and select the Shortcuts tab. Select Services from the list in the left pane of the tab, then look for the _Fast User Switch_ entry under General, ensuring the associated checkbox is selected.
1. Double-click in the area to the right of the entry, then press the desired key combination to be used to activate the user switch. (For what it’s worth, Ctrl-Option-Command + U seems to work well as a global hotkey combination.)
1. Pressing the hotkeys should display a user selection dialogue in the centre of the display. To switch to a user, select the username using the up/down cursor keys, followed by return.

## @TODO

Gracefully handle cancel action on user selection dialogue; this currently throws an error (see [issue #1](https://github.com/j13k/fast-user-switch/issues/1)).
