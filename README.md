# Wi-Fi Configuration
This app configures Android phone's Wi-Fi connection. It is suitable for administrators who want their phone users to be able to connect to Wi-Fi networks while the phone's settings app is being restricted. 

This app is only compatible with Android L (API 21) until Android P (28). It is not guaranteed to be compatible to future version of Android operating system, as Google has deprecated the Wi-Fi scanning feature since Android P.

## Features
* Turn phone's Wi-Fi radio on or off.
* Create new Wi-Fi profile (only for ESS (AP) networks with public SSID and either open security or WPA/WPA2 PSK security. Other encryption schemes such as WPA enterprise, EAP, or WEP are not supported. Networks with hidden SSIDs are also not supported).
* Connect to existing configured Wi-Fi profiles if the AP is within range (e.g. from profiles configured in settings app or by device policy controller).
* Forget (delete) Wi-Fi profiles (only for profiles created by this app).
* Automatic and continous Wi-Fi scan.
* Wi-Fi connected network indicator.

## Screenshots
![Network List](/docs/screenshot/ss1.png?raw=true)
![Saved Networks](/docs/screenshot/ss2.png?raw=true)
![Passphrase Input](/docs/screenshot/ss3.png?raw=true)

## Known Issues and Limitations
* Wi-Fi network scans is severely delayed on Android P. This is because Android P throttles Wi-Fi scanning rate for non system apps.
* This app cannot delete older profiles created by itself after the the app has been stopped for some time.

## Permissions
* `CHANGE_WIFI_STATE` and `ACCESS_WIFI_STATE` to enable turning Wi-Fi on/off and to enable network scanning and profile management.
* `ACCESS_COARSE_LOCATION` is also required to enable network scanning. This permission will be asked by system on first run on Android M or higher.