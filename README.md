# Blender AutoFocus
Per camera auto focus for Blender. Camera will auto focus on the nearest surface within the specified range.

## Installation

* Open User Preferences from the File menu and select the Add-ons tab. (File > User Preferences > Add-ons)
* Click the Install Add-on from File... button. Select the auto_focus.py file.
* Click the checkbox next to the title to enable the addon.
* Click the Save User Settings button to save your preferences.

## Usage

A new panel will be added to the bottom of the camera properties window:

<img src="https://i.imgur.com/26xcNaZ.png">

When AutoFocus is enabled, the selected camera will focus on the nearest surface directly in front of it. Only surfaces between Min and Max units from the camera will be considered.

With Smoothing enabled, the camera will focus instead on a Smooth target, which will slow-follow the AutoFocus target. This provides a smoother change in depth of field, somewhat mimicking a real camera.

The timer can be used to choose a specific update rate for the AutoFocus feature. Leaving this enabled is recommended for performance purposes. When it is disabled AutoFocus will update as often as possible, which is usually unnecessary.

Example of the AutoFocus target automatically following the surfaces of some Suzannes, with smoothing at 8.0 and a delay of 100ms:

![](autofocus.gif)
