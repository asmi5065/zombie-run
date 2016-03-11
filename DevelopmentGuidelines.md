# Introduction #

There are several things you need to know about how to code for Zombie, Run!  Some of these things are related to [Code Styles](CodeStyle.md), GPS Coordinates and specifics of writing for android.


# Code Style #

First you need to follow the coding style set in place by the rest of the code.  There are a few simple rules to follow when coding.  Please see the [Code Style](CodeStyle.md) page for more information.

# Serialization #

Data about the Zombie objects must be serialized.  This means that all variables that the zombie class contains must be able to be transfered via the Zombie::toString and Zombie::fromString methods.

This is important for two reasons:

  1. When the android interface is flipped from portrait to landscape or vice versa any data that is not serialized will be lost.
  1. When playing in multi-player only serialized data is transfered to the other players.