Mod Scorm Size
==============

The SCORM player in Moodle 2.7+ is a horror for embedded content. Why embed rather than pop up in a new window? Ipads & other tablets. They don't work properly in external windows for various iOS versions. Embeds *crop your content*. They *introduce unneccesary navigation*. They *force you to scroll* and create problems if you *resize* the window. This needs fixing.

But you can use a customscript to replace the scorm viewer with one better. Why a custom script? It's easier to update, and it's not touching core code.

![The problem](http://i.imgur.com/4y6CXOd.png)
[Click here for more images](http://imgur.com/a/d0tTU)

Installation
------------
1. Extract this to a location where you keep customscripts. I keep mine in `/local/customscripts/`
1. Change your `config.php` and include the custom script directive
    `$CFG->customscripts = __DIR__.'/local/customscripts'`

Options
-------
You can set the size of the embedded window, but there's a trick to it. You have to change the package options to 'Open in new window', which gives you control over the size. Put in the size you want the embedded content to be, noting that if the values are <= 100, they are considered to be percentages, and >100 are considered to be pixels, and that the height can't be lower than 600px (yes this is confusing: this is the unchanged default behaviour). Save the settings, and then edit the settings again. Change the open method from popup back to embedded. The size will be greyed out (but remembered), and applied to your embedded scorm package.

Versions
--------
This trick can be made to work with most Moodle versions, since the player.php code changes significantly between releases. Check the individual branches to make sure you download the version correct for you.

License
-------
GPL3
