# TP-Link Web Client
Web client for the tp-link series of smart switches (i.e. HS-100 & HS-110). Repository forked from [Andy Allsopp](https://github.com/arallsopp/tp-link-smart-switch-web-client-).

## About this application
Web client uses angular services to build a web control surface for the TP-Link series of smart plugs. TP-Link's own official app (Kasa) only runs on iOS and Android devices, so those of you with other tablets, mobiles, or desktops get left in the cold. This web client addresses that.

In use, the Kasa app generates a unique ID, then combines this with the registration information you supply at sign-up to retrieve a secure token from a TP-Link hosted API service. Requests for smart plug availability, status and relay states are sent with this token to protect your privacy.

This application is able to generate a random UUID of its own, capture your credentials, and pass these to the TP-Link hosted API service to obtain a genuine token. That token can then be used to list the devices which are present, indicate their status, and allow you to switch them on/off from anywhere you like.

Information is only sent to and from the TP-Link APIs, and is not exposed to any other server. If you opt to retain your login credentials and/or authentication token, these are stored in cookies within your browser. They are not released to me or anyone else.

To access your plugs, make sure they have remote control enabled, and are registered with the official Kasa App from TP-Link (Get Kasa here). Unfortunately, I don't know a way to perform the registration without (at least) temporary access to the official app, but once registered you can send requests from any modern browser.
