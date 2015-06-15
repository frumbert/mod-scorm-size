Mod Scorm Size
==============

The SCORM player in Moodle 2.7+ is a horror for embedded content. Why embed rather than pop up in a new window? Ipads & other tablets. They don't work properly in external windows for various iOS versions.

But you can use a customscript to replace the scorm viewer with one better. Why a custom script? It's easier to update, and it's not touching core code.

<blockquote class="imgur-embed-pub" lang="en" data-id="a/d0tTU"><a href="//imgur.com/a/d0tTU">Moodle Scorm Layout Problems</a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

Installation
------------
1. Extract this to a location where you keep customscripts. I keep mine in `/local/customscripts/`
1. Change your `config.php` and include the custom script directive
    `$CFG->customscripts = __DIR__.'/local/customscripts'`

License
-------
GPL3
