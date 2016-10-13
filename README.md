PowerShell-VSBuildTools
=======================
This PowerShell module imports and enables compiling with the visual studio commandline from powershell.  
    (This didn't exist for whatever reason, I looked long and hard. Maybe not hard enough. Sue me.)

Includes:
 - Building
 - Debugging

Based on some code orignaly found here:
https://filebox.ece.vt.edu/~ece1574/spring15/devenvinstall.html

It has been extended to be more portable and more friendly.
I am open to suggestions for better command names.

How To Use
----------
Import the module (in your PS profile or in a session)  
run get-Batchfile():  
	`Get-BatchFile('C:\Program Files (x86)\Microsoft Visual Studio 14.0\VC\vcvarsall.bat')`
	
You can now use the Visual Studio Commands yourself or use the commands provided by the module.

To change the target system, you will have to edit vcvarsall so that it defaults to your target system.  
     (Default is x86. Also note that the vcvarsall File is marked as readonly by default)
