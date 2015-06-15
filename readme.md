Mod Scorm Size
==============

The SCORM player in Moodle 2.7+ is a horror for embedded content. Why embed rather than pop up in a new window? Ipads & other tablets. They don't work properly in external windows for various iOS versions.

But you can use a customscript to replace the scorm viewer with one better. Why a custom script? It's easier to update, and it's not touching core code.

<iframe class="imgur-album" width="100%" height="550" frameborder="0" src="//imgur.com/a/d0tTU/embed?background=f2f2f2&text=1a1a1a&link=4e76c9"></iframe>

Installation
------------
1. Extract this to a location where you keep customscripts. I keep mine in `/local/customscripts/`
1. Change your `config.php` and include the custom script directive
    `$CFG->customscripts = __DIR__.'/local/customscripts'`

License
-------
GPL3
