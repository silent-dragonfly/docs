# Connection initiation

## Searching Access Points

First step of Wi-Fi Station (or end-device) is finding available Access Points.
To do that Station can send broadcast **probe-request** with list of supported
standards, and Access Point can answer **probe-response** with SSID if it has at least
one of supported standard. This method called **active scan**.

On the other side, Access Point periodically sends **Beacon frame** with
advertisement of wireless network. And Station can listen this packets to make
a list of available networks.

## Authentication and Association

After Station (STA) find appropriate Access Point (AP) to communicate it should
come through tree satages:

1. Unauthenticated and Unassociated
1. Authenticated, Unassociated
1. Authenticated, Associated

In other words STA should authenticate and then associate with AP:

1. STA -> AP: **Authentication Request**
1. AP -> STA: **Authentication Response**
1. STA -> AP: **Association Request**
1. AP -> STA: **Association Response**

**Important Note**: that authentication were designed for WEP encryption, which
currently has been proven insecure, so in most cases that process goes with
*Open System Authentication* (NULL authentication) for backward compatibility.
WPA/WPA2 or 802.11X authentication as a keys exchange goes after this process.


<font color="red">TODO: add details about 802.11 considered frames format</font>

### References

- Web article: [Association process](https://wifibond.com/2017/04/08/802-11-association-process/)
- Web article: [Association process explained](https://documentation.meraki.com/MR/WiFi_Basics_and_Best_Practices/802.11_Association_process_explained)
- [Wiki:IEEE 802.11i-2004](https://en.wikipedia.org/wiki/IEEE_802.11i-2004)