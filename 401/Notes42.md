# Location

The Google Location Services API, part of Google Play Services, provides a more powerful, high-level framework that automates tasks such as location provider.

Google provides 5 user states which are In Vehicle, On Bicycle, On Foot, Still, and Tilting, which are good enough to detect user’s activity, and to provide right content according to user’s status.

The Google Play Services Location API can request the last known location of the user’s device, this is equivalent to the user’s current location.

To get the device’s last known location, use the FusedLocationProviderApi which allows you to specify requirements such as the location accuracy required. High accuracy means more battery power used.

Priority :

setPriority() - This method sets the priority of the request, which gives the Google Play services location services a strong hint about which location sources to use , supported values :

1. PRIORITY_BALANCED_POWER_ACCURACY

2. PRIORITY_HIGH_ACCURACY

3. PRIORITY_LOW_POWER

4. PRIORITY_NO_POWER

Allow your users to explore the world with rich maps provided by Google , The Google Maps Android API allows you to include maps and customized mapping information in your app.