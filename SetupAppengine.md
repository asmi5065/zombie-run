# Introduction #

This is a guide to help getting started on using AppEngine and working on Zombie, Run! 2 (Zombie, Run! in HTML for Android and iPhone).  This is not meant to be exhaustive but simply a quick cheat sheet guide to getting up and running as quickly as possible.

# An email brain dump #

Get the AppEngine SDK for Python: http://code.google.com/appengine/downloads.html#Google_App_Engine_SDK_for_Python
Checkout and update the ZombieRun repository: http://code.google.com/p/zombie-run/source/checkout

From the repository directory (the one containing GameServer, Website, etc), run:

> dev\_appserver.py GameServer --address=localhost --enable\_sendmail

You can change --address=localhost to (for instance) --address=peterdolan-macbookpro.local if you would like the server to be available on your local network.  I use that to develop on my iPhone or Android devices, just load http://peterdolan-macbookpro.local:8080/ in your phone.

You should be able to create an AppEngine instance and upload the server, just don't spread any public URLs around.  We'll eventually launch this at game.zrli.org (where you can see a dev version at the moment) or zombierun.zrli.org.  Don't spread those URLs around yet, though.