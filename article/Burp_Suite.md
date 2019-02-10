# Burp Suite

Personal notes for installing and using Burp Suite.

## Installing Burp Suite

Download Link: [[+]](https://portswigger.net/burp/communitydownload)

Naviagte to the location where the file was downloaded and run the bash script:

`sudo bash burpsuite_community_linux_v1_7_36.sh`

Done! Navigate to Burp Suite and Launch

## Setting up Burp Suite with Firefox

Open Firefox and click the Menu button near the top right of the window. _Looks like a hamburger_

Once in the menu, in the `General` section, scroll to the bottom of the page and click on `Settings` under the `Network Settings` section.

In the `Connection Settings` pop-up window, select the option that reads `Manual proxy configuration` and fill in this information:

- HTTP Proxy`127.0.0.1` Port`8080`
- Use this proxy server for all protocols

Head over to Burp Suite and click on the `Options` tab under the `Proxy` menu.

Ensure that the Proxy Listener on the interface `127.0.0.1:8080` is running.

If no interface exists, click `Add` and populate the fields with these values and ensure it is running:
```
Bind to port:`8080`
Bind to address: Loopback only
```
