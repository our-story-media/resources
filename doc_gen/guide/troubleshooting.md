---
title: Troubleshooting
---

# Troubleshooting

## Dashboard

### Sharing Your Log File

Indaba Dashboard has a log which can be used to diagnose many issues. To access the log, Insert a USB drive into the Dashboard Kit, wait a few seconds and then pull out the USB device. This will have copied a log text file to the USB drive which you can copy and share to help diagnose problems.

<!-- ### Installation Hangs / Not doing anything

When using the `Toolbox` version of Indaba (which is backed by Docker Toolbox), there are sometimes issues where Docker fails to start. Often the easiest method of getting it going again is to:

- Reboot the machine
- Changing the network whilst docker is 'hung' often triggers it to continue.
- Trying to start Indaba for the first time whilst connect to the internet (in theory it does not need to download anything but this sometimes makes it work). -->
<!--
### Network Wont Reconnect After Closing Dashboard

Run the `Fix Network` tool installed alongside Indaba Dashboard. -->

## Story Publishing

### Videos are not the right Length

Sometimes the device that recorded the original video does not report the length correctly, and this causes issues with the story publishing step. This can be easily rectified by following these steps:

- Clone the story that has the issues
- Open the story in editor the Android application
- Press the `Trim` and then `Back` button for each video in the story in turn. (this overrides the reported length)
- Save the story and publish again

### Errors

**Error 1: No network connection**
This error signifies that the device does not have a WiFi (or 3G) connection.

**Error 2: Cannot connect to application**

**Error 3: Invalid API Key**

**Error 4: We are having trouble retrieving your information. Login again to continue**

**Error 5: Please try logging in again**

**Error 6: Request cancelled by participant**

**Error 7: Server error**

**Error 8: Unknown Network Error**

### Connection Screen

The connection screen has a list of 4 checks that the app makes when starting up. These checks can help you diagnose potential issues with your Indaba setup.

- **WiFi Connected**: This checks if you have an active WiFi connection which the phone is connected to. If this is not ticked, check the device is connected to your local Indaba network.
- **IP Address Range Correct**: This checks if the network it is connected to is setup for Indaba, where it gets allocated an IP address in the range 10.10.10.x. If this is not ticked, check which WiFi is connected and check that this WiFi is the Indaba one.
- **Remote Application Found**: This checks that the Dashboard computer can be found on the WiFi network. If this is not ticked, check your computer is on, connected to the Indaba WiFi and has configured it's IP address correctly.
- **Connection Established**: This checks that communication with the Dashboard is possible. If not ticked, check that the Dashboard application is running on your computer and restart if necessary.
