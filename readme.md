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

License
-------
GPL3
