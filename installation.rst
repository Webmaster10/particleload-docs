Installation
======================

Extract ParticleLoad
----------------------------------
After you have downloaded ParticleLoad, extract the "INSTALL" folder from the ParticleLoad zip file to somewhere on your computer, preferably your desktop for easy access.

Getting Your Steam API Key
----------------------------------------
Before installing ParticleLoad, you will need to head over `here <https://steamcommunity.com/dev/apikey>`_ to get your Steam API key. If you have not already filled in this form, do so now to get your Steam API Key.

Entering Your Steam API Key
-----------------------------------
Now, open up the "INSTALL" folder you previously extracted, and edit the file called "config.php". Where you see the line: ::

    $steamAPIKey = "";

Enter your Steam API Key between the two quotation marks and save your changes.

Changing the Admin (Optional)
----------------------------------
By default, the admin is the person who purchased ParticleLoad on ScriptFodder. If for some reason you want to change this, change the Steam ID in config.php next to $admin. Note that this must be a SteamID64 i.e.
"76561198134262586" and NOT a SteamID32.

Upload To Your Web Host
----------------------------
Your web host will have a folder called something like "public" or "public_html". Create a folder in here, for this guide I will call  this folder "loadingscreen" from here on. Now upload all of the files from
INSIDE the extracted "INSTALL" folder to the "loadingscreen" folder using FTP or your web host's built-in file browser.

ParticleLoad is now installed and you can move onto the configuration stage.
