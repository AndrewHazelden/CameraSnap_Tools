CameraSnap.mel

Version:  1.0
Creation Date:  March 28, 2013

Author:
Andrew Hazelden

Contact:
andrew@andrewhazelden.com
http:www.andrewhazelden.com


About the Script:
CameraSnap.mel takes a list of selected cameras in your scene as an input and creates a new camera with an animation path that moves through the position of each of the original input cameras.

The script was created to convert the dozens of still cameras imported from a photogrammetry program like Autodesk 123D Catch into a single camera animation path.

This script could also be used for converting a matrix style time-slice rig aka. "bullet-time" camera rig in your Maya scene into a single camera with a path animation that can be playedback in the viewport and controlled using Maya's normal time controls. 



CameraSnap.mel Script Installation:

Windows MEL Script Install:

To load the CameraSnap.mel script in Maya copy the MEL script file to your user account's Maya scripts folder.

On Windows the script folder is located in the folder:
My Documents\maya\<maya version number>\prefs\scripts

In this case <maya version number> is a placeholder for your actual Maya release number like "2013-x64". 

Copy the shelf tool to the Maya Shelves folder:
My Documents\maya\<maya version number>\prefs\shelves

Copy the icons to the Maya Shelves folder:
My Documents\maya\<maya version number>\prefs\icons


------------------------------------------------------------

Mac OS X MEL Script Install:

To load the CameraSnap.mel script in Maya copy the MEL script file to your user account's Maya scripts folder.

On mac os X the folder is located in your preferences folder.
~/Library/Preferences/Autodesk/maya/<maya version number>/prefs/scripts

In this case <maya version number> is a placeholder for your actual Maya release number like "2013-x64".

You can open the hidden Library folder on Mac OS X by using the Finder > Go to Folder menu item. Paste in the value:
~/Library/Preferences/Autodesk/maya/ and hit the "go" button.

Copy the shelf tool to the Maya Shelves folder:
~/Library/Preferences/Autodesk/maya/<maya version number>/prefs/shelves

Copy the icons to the Maya Shelves folder:
~/Library/Preferences/Autodesk/maya/<maya version number>/prefs/icons

------------------------------------------------------------

Usage:
Select a group of cameras in the outliner or a viewport. Click the Camera Snap icon in the shelf to create a new animated camera that will move through the position of each of the input cameras in the original camera 'array'.

The output duration of the new camera rig animation is based upon the total number of cameras in the original selection. By default the new camera animation path is set to use linear tangents.

Note:
If you adjust the near clipping distance the for new camera, the motion trail handle control knots might become visible in the masterCamera1 camera view. In this case you can manually hide the motion trail before you play the camera animation back.
