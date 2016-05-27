Configuration
=======================

Accessing the Configurator
------------------------------------
To access the settings page, go to http://<yourdomain.tld>/<particleloadfolder>/settings.php

For example, if your domain name is "myamazingdomain.com" and the folder you put ParticleLoad in is called "loadingscreen", go to http://myamazingdomain.com/loadingscreen/settings.php

You will be presented with a Steam login page, sign in with your Steam account to continue.

.. note::
    Only the Steam account defined in config.php next to $admin will be able to log in to the configurator. By default this is the account that purchased ParticleLoad on ScriptFodder. Instructions for changing this can be found in the
    "Installation" section of the documentation.

Setting sv_loadingurl
-------------------------------------------------
To apply the loading screen on your Garry's Mod server, edit your server.cfg, if it doesn't already add a line starting with "sv_loadingurl" (without quotation marks), then a space, then in quotation marks
copy the Loading URL from the top of the ParticleLoad settings page. For this example, it would look like: ::

    sv_loadingurl "http://myamazingdomain.com/loadingscreen/index.php?steamid=%s"

When you have done this save your settings and restart your Garry's Mod server.

Replacing/Deleting the Logo
---------------------------------------
ParticleLoad can display a logo of your choice above the loading screen content. You can use this to, for example, display your server or community's logo. To replace it, on your web host go into the folder
you installed ParticleLoad in ("loadingscreen"), then go into the "img" folder, then the "logo" folder. Delete the image file already in here to remove the default logo, then if you want, upload your own image
file to replace it. It doesn't matter what you call this file, ParticleLoad will use the first file it finds.

.. note::
    ParticleLoad supports any image file that is capable of being displayed in modern web browsers including jpeg, png, gif, svg and bmp.

Editing the Loading Screen's Appearance
-------------------------------------------------
The first thing you will see when you open ParticleLoad's settings page is the appearance tab. Here you can customise almost every aspect of ParticleLoad's appearance, settings are grouped into categories to make
it easier to find the thing you want. Feel free to experiment with things here - you can always hit the "Reset" button at the bottom right to reset everything back to default settings (this will not reset cards you've added or music settings).
Hit the "Save" button at the bottom-left to save your settings, then press the "Preview" button at the top to see how everything looks.

Adding/Editing cards
------------------------
The main content of ParticleLoad is defined in "Cards", which ParticleLoad will automatically transition between. To access the cards settings, click on the "Cards" tab at the top. Cards are extremely simple to set up, and to give you an idea
of how they work ParticleLoad comes with a few cards already set up. To add a card, click on the "Add Card" button at the bottom right. A menu will appear asking you to select a card type, the types of cards are as follows:

Server Info - Text
    This will show the user's Steam avatar, then below it will display some text of your choice containing information about the server. Use placeholder phrases such as %servername% (more info on these below) to display information about the
    server.

Server Info - List
    This is similar to a "Server Info - Text" card, but instead of a paragraph of text it will display a list of information about the server along with icons to the left as well as some text of your choice above it.

List - Numbered
    This will create a list in the form of a table with the numbers at the left and list items to the right. You can edit the list items and add as many items as you desire. This is ideal for creating a rules list for your server.

List - Non-Numbered
    This will create a list of items (without numbers) seperated by dividers. Again, you can edit the list items and add as many items as you desire.

Text
    This will allow you to enter whatever you want to displayed, including text and images. Advanced users can even enter their own HTML.

To edit a card's contents, click on the pencil icon beside it. This will open an editor which will look different depending on the type of card. For most types of card this will be a text editor where you can enter what you want, but for list
cards this will be a list editor where you can add, edit and remove list items. All types of card support placeholder phrases such as %servername% (more info on these below).

Placeholder Phrases
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Placeholder phrases are simply phrases that are replaced by server information when a user connects to the server. For example, the "%servername%" placeholder will be replaced by the servers name, so if I put in a card's content "Hello, and
welcome to %servername%", and my server's name was "MyAmazingServer", when a user connects that would become "Hello, and welcome to MyAmazingServer". All of the valid placeholder phrases are as follows:

* **%servername%** - The server's name
* **%username%** - The user's Steam username
* **%gamemode%** - The gamemode the server is currently playing
* **%mapname%** - The full name of the map the server is currently playing
