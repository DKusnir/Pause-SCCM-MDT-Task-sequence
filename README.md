# Pause-SCCM-MDT-Task-sequence
GUI to pause the SCCM / MDT task sequence


There are a countless methods how to pause the task sequence - this is one of them. It is a simple GUI with a progress bar , that will hide the task sequence progress bar and allow you to test the programs / scripts ...etc before the task sequence ends. In order to use this in the WinPE, you must enable .net in the boot image

![ScreenShot](https://github.com/DKusnir/Pause-SCCM-MDT-Task-sequence/blob/master/Picture.png)

In order to make this work, you have to do the following : 

1. create a package 

2. Add Run command line 

3. Command line: wait.exe . 

4. In case you need to open up cmd, modify command:  wait.exe /cmd

5. point to the right package ( in case of the SCCM ) 

![ScreenShot](https://github.com/DKusnir/Pause-SCCM-MDT-Task-sequence/blob/master/SCCM.JPG)

==========================================

Version 1.0.0.6 - Add Dark Flat theme

Version 1.0.0.5 - Fix CMD and PowerShell opening in the WinPE. Fix check for updates

Version 1.0.0.4 - Added Tools menu strip to open up CMD line and PowerShell console. Added High-DPI Awarness. Added Check for Updates. Added ability to skip Pause using variable SkipPause = True

Version 1.0.0.3 - Added simple timer to show elapsed time for TS pause. Added switch "/cmd" to auto open commandline for images without F8 support.

Version 1.0.0.2 - Added Top most. Added GUI close via Enter & Esc. Compiled versions for Win 7 and Win 10

Version 1.0.0.1 - Initial release
