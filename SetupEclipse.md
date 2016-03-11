# Introduction #

This is a guide to help getting started on using Eclipse and working on Zombie, Run!.  This is not meant to be exhaustive but simply a quick cheat sheet guide to getting up and running as quickly as possible.

# Getting started #

First follow the instructions on the Google Android setup page.  (Example: http://developer.android.com/sdk/1.5_r1/installing.html).  This typically works as advertised.

Some possible issues:
  * Change the available software site from https://dl-ssl.google.com/android/eclipse/ to http://dl-ssl.google.com/android/eclipse/ (Notice http, not https)
  * If you have gcj (Gnu Java Compiler) you will need to install the sun java.  For debian: make sure you have non-free in your apt/sources.list file and then **apt-get install sun-java6-jdk sun-java6-jre**.  Then run **update-alternatives --config java** and choose the new Sun package.
  * Note: with the 1.5 SDK I received some problems about Android Ping and something about a crash.  Just ignore that and continue... everything seems to work fine.  My understanding is that is a check for Usage statistics and is not important.

# Load the project #

After you have downloaded the code via svn you can load the project into Eclipse.

  1. File->New->Other...   (or CTRL+N)
  1. Android->Android Project (click Next)
  1. Choose Create Project from Existing Source
  1. Choose the base directory for ZombieRun from the SVN checkout repository.  This should be the directory that contains the AndroidManifest.xml file.
  1. Set the Project Name to ZombieRun and pick the SDK build target. **You must pick Google API**.  With v1.5 of the SDK the maps API is seperate.  Picking Google API will include 1.5 and the the mapping libraries.

This should load the project up in your editor.

## Troubleshooting ##

**errors when including com.google.android.maps...**

This is because the new SDK requires the Google APIs to be listed as a build target.  To modify (or upgrade) your project after getting the latest SDK you can right click on your project name in Package Explorer and choose Properties.  Here you can modify your build target.