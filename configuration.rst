Configuration
=======================

Accessing the Configurator
------------------------------------
To access the settings page, go to http://<yourdomain.tld>/<particleloadfolder>/settings.php

For example, if your domain name is "myamazingdomain.com" and the folder you put ParticleLoad in is called "loadingscreen", go to http://myamazingdomain.com/loadingscreen/settings.php

You will be presented with a Steam login page, sign in with your Steam account to continue.

.. note::
    Only the Steam account defined in config.php next to $admin will be able to log in to the configurator. By default this is the account that purchased ParticleLoad on ScriptFodder. Instructions for changing this can be found in the "Installation" section of the documentation.

Replacing/Deleting the Logo
---------------------------------------
ParticleLoad can display a logo of your choice above the loading screen content. You can use this to, for example, display your server or community's logo. To replace it, on your web host go into the folder you installed ParticleLoad in ("loadingscreen"), then go into the "img" folder, then the "logo" folder. Delete the image file already in here to remove the default logo, then if you want, upload your own image file to replace it. It doesn't matter what you call this file, ParticleLoad will use the first file it finds.

.. note::
    ParticleLoad supports any image file that is capable of being displayed in modern web browsers including jpeg, png, gif, svg and bmp.

Editing the Loading Screen's Appearance
-------------------------------------------------
The first thing you will see when you open ParticleLoad's settings page is the appearance tab. Here you can customise almost every aspect of ParticleLoad's appearance, settings are grouped into categories to make it easier to find the thing you want. Feel free to experiment with things here - you can always hit the "Reset" button at the bottom right to reset everything back to default settings (this will not reset cards you've added or music settings). Hit the "Save" button at the bottom-left to save your settings, then press the "Preview" button at the top to see how everything looks.

Background Images/Slideshow
---------------------------------
To use an image as the background, or use a set of images in a slideshow as the background, go into the folder you installed ParticleLoad in ("loadingscreen"), then go into the "img" folder, then the "background" folder. Upload any images you want to use in here. If you upload one, ParticleLoad will use that image as the only background, and if you upload multiple, it will use all of them in a slideshow. ParticleLoad automatically detects the images you upload so it doesn't matter what you name them, however it will play the images in the slideshow in alphabetical order of their filenames. The slideshow is also synced with the card animations.

Adding/Editing cards
------------------------
The main content of ParticleLoad is defined in "Cards", which ParticleLoad will automatically transition between. To access the cards settings, click on the "Cards" tab at the top. Cards are extremely simple to set up, and to give you an idea of how they work ParticleLoad comes with a few cards already set up. To add a card, click on the "Add Card" button at the bottom right. A menu will appear asking you to select a card type, the types of cards are as follows:

Server Info - Text
    This will show the user's Steam avatar, then below it will display some text of your choice containing information about the server. Use placeholder phrases such as %servername% (more info on these below) to display information about the server.

Server Info - List
    This is similar to a "Server Info - Text" card, but instead of a paragraph of text it will display a list of information about the server along with icons to the left as well as some text of your choice above it.

List - Numbered
    This will create a list in the form of a table with the numbers at the left and list items to the right. You can edit the list items and add as many items as you desire. This is ideal for creating a rules list for your server.

List - Non-Numbered
    This will create a list of items (without numbers) seperated by dividers. Again, you can edit the list items and add as many items as you desire.

Text
    This will allow you to enter whatever you want to be displayed, including text and images. Advanced users can even enter their own HTML.

To edit a card's contents, click on the pencil icon beside it. This will open an editor which will look different depending on the type of card. For most types of card this will be a text editor where you can enter what you want, but for list cards this will be a list editor where you can add, edit and remove list items. All types of card support placeholder phrases such as %servername% (more info on these below). You can change the order cards will show up in by pressing the arrow icons at the left to switch their order. Remember to hit the "Save" button to save your changes.

Placeholder Phrases
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Placeholder phrases are simply phrases that are replaced by server information when a user connects to the server. For example, the "%servername%" placeholder will be replaced by the servers name, so if I put in a card's content "Hello, and welcome to %servername%", and my server's name was "MyAmazingServer", when a user connects that would become "Hello, and welcome to MyAmazingServer". All of the valid placeholder phrases are as follows:

* **%servername%** - The server's name
* **%username%** - The user's Steam username
* **%gamemode%** - The gamemode the server is currently playing
* **%mapname%** - The full name of the map the server is currently playing

Adding/Editing Music
---------------------------------
ParticleLoad is capable of playing music from YouTube videos and directly from .ogg music files. To access the music settings, click on the "Music" tab at the top. When making any changes remember to hit the "Save" button.

.. note::
    If you have MP3, WAV, FLAC etc. files that you want to use with ParticleLoad, they will need to be converted to OGG format. You can use websites such as http://media.io/ to do this, just be sure to select OGG as the output format.

Music settings
^^^^^^^^^^^^^^^^^^^^^^^^
There are several settings on the Music tab. The purpose of these is as follows

Music Enabled
    This simply enables or completely disables Music playback. If you can't hear your music make sure this is on.

Music Play Order
    This is the order the music will be played in. If set to "Sequential" the music will be played in the order you set it to play in, and if set to "Random" it will mix up the order.

Play Music Again When Playlist Finishes
    If this is set to on, the playlist will start over again when all songs have been played, and if it is set to off the music will turn off when all songs have been played.

Music volume
    This simply sets the volume of the music on a scale of 0-100 - 0 being silent and 100 being full volume.

Adding Music From a YouTube Video
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
To add a song from a YouTube video, click on "Add Song" at the bottom-right and select "YouTube Video" as the source. Enter the song's name and artist in the respective fields then enter the URL to the video. Once you have done this, click on the "Test" button to make sure it is working. If it is working, the video will appear below and you can play it, and if it is not working it will display a YouTube error image and you cannot play it. If it is not working, make sure there are no errors in the URL and try again. When it is working hit "Add Video".

Adding Music From an OGG File
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Adding music from an OGG file is a bit trickier but still very easy. You will need to upload your .ogg file into the "music" folder in the folder on your web host you installed ParticleLoad in, then refresh the settings page. Now, click on "Add Song" and select "OGG File" as the source. Enter the song's name and artist, then select the filename that matches the one you just uploaded from the selection, then hit "Add Song".

Setting the Music Play Order
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
To change the order the music plays on, click on the small arrows next to the songs to change their order, then hit the "Save" button to save your changes.

.. note::
    If you set the Music Play Order to "Random" this order will be ignored and songs will instead be played in a random order.
