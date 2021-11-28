ADD Z-WAVE DEVICES UNSECURE

Z-wave associations are a very important. The main reason is that if Homey isn’t working for some reason, the lights can still be controlled.

As of version 7.0, Homey supports more z-wave security levels. That is great for locks and such, but not so much for z-wave associations, because associations need the same security level for both devices in order to work.

As not all devices support the same security level, and Homey picks the security level based on the devices capabilities, associations are basically broken now if both devices have different security levels. That is why it is important that users are able to select a lower security level for devices that do not require premium security, so they can pick the level that both devices support.

The way this app works is inspired on a workaround that used to exist before Homey version 7.0, which was to pick a Walli device for pairing, even though the device you want to add is not a Walli. This would force the device to be added unsecure. This app works in the same way, but now for version 7.0 and higer firmwares for Homey.

First make sure you have the proper app for your z-wave device istalled on your Homey. That is because you still need the real driver to operate the device. But here's the trick. When adding the device to Homey, pick UnZ-cure as the device to pair, instead of the z-wave device it actually is. 

Don't worry: Homey will still add the device as the right type, from the right app. The UnZ-cure will just add a parameter to prevent z-wave secure inclusion. Also, unsecure inclusion is not as unsecure as it seems. Sure, secure is more secure, but it still requires a lot of effort to hack your lights if you're adding it unsecure.