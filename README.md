Inactive Panes
==============

Inactive Panes is a plugin for [Sublime Text][st] 2 and 3 that will dim the currently inactivate panes to show you more visibly where your cursor is and which view is focussed. Really Useful with the [Origami][origami] plugin or ST3's native panel handling.

This plugin is still *beta* but you are more than free to test it. Please report errors you encounter with this plugin [here][issues].

**Warning**: Do not use this with other color-changing plugins like [LiveCSS][livecss] as it will probably cause various issues and eventually *bring the world to an end*.


Originally created by [adzenith][adzenith], maintained by [FichteFoll][FichteFoll].


Usage
-----

It will automatically dim inactive groups when you install it.

When you want to disable this package, the easiest solution is to simply set the dim strength to `0`.
Alternatively you can use Package Control's `Disable Package` and `Enable Package` commands.

**Warning**: If you want to remove the package, use Package Control's `Remove Package` command. Do **not** delete the plugin folder by yourself if you didn't disable the package before! This will cause various error messages (but nothing critical).

### Configuration

The following settings can be modified in your User settings file (`Preferences > Settings - User`):

*   `"inactive_panes_dim_color"` (*default*: `"#7F7F7F"`, gray)

    Change the color to dim to.

*   `"inactive_panes_dim_strength"` (*default*: `0.2`)

    Change the dim strength; ranges from `0` (no modification) to `1` (everything will be changed to the color set above).

### Screnshots

#### Dark Scheme

Using [a modified][tw-fichte] Twilight color scheme with a dim strength of `0.1`:

[![][scr-dark-thumb]][scr-dark]

#### Bright Scheme

Using LAZY color scheme with a dim strength of `0.3`:

[![][scr-bright-thumb]][scr-bright]

#### Custom Color

Using [a modified][tw-fichte] Twilight color scheme with a custom color of `"#7F7F00"` and dim strength of `0.1`:

[![][scr-dark_colored-thumb]][scr-dark_colored]


### Known Issues

- When opening the same file in two groups (with command palette or by cloning it) both of the views will be marked as active. This is because there is no way to assign different color schemes to these view's since they share the same settings.


Install
-------

### Package Control

You can install this package from [Package Control][pck-ctrl] under `"InactivePanes"`.

### Alternative

Browse the [Packages][packages-dir] sub-folder of your [Data directory][data-dir] and clone the repo:

    git clone git://github.com/SublimeText/InactivePanes.git

Alternatively you can download a recent [zip archive][tags] and extract it into an "InactivePanes" sub-directory of the Packages dir mentioned above.


About
-----

Inactive Panes is a split from [Origami][origami] which once included this feature but due to various (unfixable) issues it was removed. I extracted relevant commits from the Origami repo to keep developing this feature because I've used it ever since (with no issues yet) and think that it's really useful.


[st]: https://www.sublimetext.com/
[origami]: https://github.com/SublimeText/Origami
[issues]: https://github.com/SublimeText/InactivePanes/issues
[livecss]: https://github.com/a-sk/livecss

[adzenith]: https://github.com/adzenith
[FichteFoll]: https://github.com/FichteFoll

[tw-fichte]: https://gist.github.com/FichteFoll/5522507 "Gist: Twilight-Fichte.tmTheme"
[scr-dark]: http://i.imgur.com/4uKGLf3.png "Twilight color scheme; 0.1"
[scr-dark-thumb]: http://i.imgur.com/4uKGLf3l.png
[scr-bright]: http://i.imgur.com/CCcl1v3.png "LAZY color scheme; 0.3"
[scr-bright-thumb]: http://i.imgur.com/CCcl1v3l.png
[scr-dark_colored]: http://i.imgur.com/m5rc8j9.png "Twilight color scheme; 0.08; #7F7F00"
[scr-dark_colored-thumb]: http://i.imgur.com/m5rc8j9l.png

[pck-ctrl]: http://wbond.net/sublime_packages/package_control "Sublime Package Control by wbond"
[data-dir]: http://docs.sublimetext.info/en/latest/basic_concepts.html#the-data-directory
[packages-dir]: http://docs.sublimetext.info/en/latest/basic_concepts.html#the-packages-directory
[tags]: https://github.com/SublimeText/InactivePanes/tags "Tags - SublimeText/InactivePanes"
