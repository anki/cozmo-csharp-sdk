# cozmo-csharp-sdk
Anki Cozmo C# SDK Interface

Unlike the Cozmo Python SDK - https://github.com/anki/cozmo-python-sdk - the C# SDK is not actively maintained by Anki, and is instead meant as starting point for anyone who wishes to build their own C# SDK for interacting with Cozmo.

We will release an updated CladCSharp.dll for each subsequent release of the Cozmo app, so that you don't need to worry about the binary format of the messages when they're sent over the network.

The Cozmo Python SDK GitHub repo: https://github.com/anki/cozmo-python-sdk

Learn more about Cozmo: https://anki.com/cozmo

Learn more about the SDK: https://developer.anki.com/

SDK documentation: http://cozmosdk.anki.com/docs/

Forums: https://forums.anki.com/



The included project can be built on macOS via Xamarin Studio, or on Windows via Visual Studio. This project is a very small sample application which demonstrates how to send an action to Cozmo, and how to register for specific callbacks to receive incoming messages.  Other messages can be found by browsing the CladCSharp.dll assembly, and can be send and listened for using a similar approach.

To connect to the Cozmo app running on your mobile device, you will need to plug in the device via a USB cable, and also set up port forwarding for TCP port 5106 to go over the USB cable.

For Android devices use adb:

adb forward tcp:5106 tcp:5106

For iOS devices you will need to use the usbmux protocol (usually installed as part of iTunes) along with something like libimobiledevice.
