# Device ID checker

This app checks the MAC address, BSSID (the MAC address of your router), and Android ID with minimal permissions. If this app displays your MAC address and BSSID, it means that your OEM may allow apps to access such information for all apps. This can be a major privacy issue. I will release various apps with at least `ACCESS_NETWORK_STATE` and `ACCESS_WIFI_STATE` permissions. In other releases I will publish other APKs with varying degrees of permissions enabled as even declining a permission will still allow them to get partial use.

Many apps passively collect such information to build a profile on you. If you want to learn more about permission of apps check out exodus-privacy.eu.org/ there you can query all sorts of apps and their permissions. 


# Future

I will soon release a ADB script which disables these dangerous permissions and another for a specific OEM(s) and their hidden APIs.
