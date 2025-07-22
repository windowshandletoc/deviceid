# Device ID checker

This app checks the MAC address, BSSID (the MAC address of your router), and Android ID with minimal permissions. If this app displays your MAC address and BSSID, it means that your OEM may allow apps to access such information for all apps. This can be a major privacy issue. I will release various apps with at least `ACCESS_NETWORK_STATE` and `ACCESS_WIFI_STATE` permissions. In other releases, I will publish other APKs with varying degrees of permissions enabled, as even declining a permission will still allow them to get partial use.

Many apps passively collect such information to build a profile of you. If you want to learn more about the permissions of apps, check out [Exodus Privacy](https://exodus-privacy.eu.org). There, you can query all sorts of apps and their permissions. 


# Future

I will soon release an ADB script that disables these dangerous permissions and another for a specific OEM(s) and their hidden APIs.

# Update

Current releases marked as pre-release will almost certainly return a dummy value. I will make new releases that will display the BSSID and MAC of the current device. For BSSID, I am sure that it will work for all devices. For the MAC address of the device it may vary among manufacturers. Having any app that has location and WIFI permission (`ACCESS_COARSE_LOCATION`, `ACCESS_WIFI_STATE`, and sometimes `ACCESS_FINE_LOCATION`), even if disabled through settings on the device, may leak BSSID and MAC address. This data is often collected by data providers and anti-fraud libraries, and SDKs.
