GMusic-beets-plugin
===================

A simple GMusic plugin for beets.

This adds "gmusic-upload" and "gmusic-query" commands to beets. 

##Features

* Upload songs from your beets library to Google Music

* Search for songs in your Google Music library

##Installation

Just move the "GMusic-beets-Plugin" folder to your "beetsplug" folder and add "gmusic-upload" and "gmusic-query" to your .beetsconfig file.

##Usage

beet gmusic-upload [beets query]

For example, to upload all of the songs by the band "Foo Bar", just use
beet gmusic-upload -p [your password] -u [your username] artist:Foo Bar

beet gmusic-query [Google Music song query]

For example, to search for the song "Foo Bar", just use
beet gmusic-query -p [your password] -u [your username] -q "Foo Bar"

##Arguments

* -a, --aggressive: The plugin will not ask for confirmation when uploading songs.
* -p, --password: Your Google account password.
* -t, --TagWithSID: Tags uploaded songs with the Google Music SID. This is not used for anything yet, and modifies your music files. Please don't use this option right now.
* -u, --username: Your Google account username.

##More Information

This plugin uses the Unofficial Google Music API to interact with Google Music.
The Unofficial Google Music API can be found at https://github.com/simon-weber/Unofficial-Google-Music-API



