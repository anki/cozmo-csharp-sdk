# cozmo-csharp-sdk
Anki Cozmo C# SDK Interface

**Please note that updates to this C# SDK interface are indefinitely on hold. Current users can continue to use it, though must remain on version 3.0 of the Cozmo mobile app.**

Unlike the Cozmo Python SDK - https://github.com/anki/cozmo-python-sdk - the C# SDK is not actively maintained by Anki, and is instead meant as starting point for anyone who wishes to build their own C# SDK for interacting with Cozmo.

The Cozmo Python SDK GitHub repo: https://github.com/anki/cozmo-python-sdk

Learn more about Cozmo: https://anki.com/cozmo

Learn more about the SDK: https://developer.anki.com/

SDK documentation: http://cozmosdk.anki.com/docs/

Forums: https://forums.anki.com/



The included project can be built on macOS via Xamarin Studio, or on Windows via Visual Studio. This project is a very small sample application which demonstrates how to send an action to Cozmo, and how to register for specific callbacks to receive incoming messages.  Other messages can be found by browsing the CladCSharp.dll assembly, and can be sent and received using a similar approach.

To connect to the Cozmo app running on your mobile device, you will need to plug in the device via a USB cable, and also set up port forwarding for TCP port 5106 to go over the USB cable.

For Android devices use adb:

adb forward tcp:5106 tcp:5106

For iOS devices you will need to use the usbmux protocol (usually installed as part of iTunes) along with something like libimobiledevice.
