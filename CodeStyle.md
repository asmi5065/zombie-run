# Introduction #

Here is a brief coding standard that you should adhere to when coding for Zombie, Run!

  * All lines less than 100 characters long.
  * Spaces between arithmetic operators.
  * Curly braces on the same line as if- or loop-statements.
  * Indent using two spaces, not with tabs.

In Eclipse, the tabs can be set to two spaces by going to:

Window->Preferences
> General->Editors->Text Editors
> > Display Tab Width: 2

# Example #
```
// if we are at our location or 10% chance of change direction
if (location == targetDirection || Math.floor(Math.random() * 100) < 10) {
  targetDirection = GeoPointUtil.getGeoPointNear(location, 804.67200); // Half a mile
} else {
  location = GeoPointUtil.geoPointTowardsTarget(location, targetDirection, movementDistanceMeters);
}
```