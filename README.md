# XexTool
This is the last version of Xorloser's XexTool, released in 2013.
Since I only see version 6.3 online, and I have that version, I'm uploading it here.

This is a tool to extract information on an xex file. It will print out xex information to the console, alter xex attributes, extract executable code and other basefiles and create idc scripts files to help with disassembling the extracted executable code.



:: Install

If you wish to run xextool from anywhere, copy the xextool.exe file to
a location in your path that is used for exe files. If you are not sure
you can check the %PATH% environment variable (type "echo %PATH%" from
the command line) or just copy it into your windows directory.

If you use the "Create IDC" feature of xex tool then you need to copy
x360_imports.idc into your "IDA\idc" directory so that it will be found
by any IDC script that you run.


:: History

v6.6
	* fixed printing of library versions
	
	+ added an option to remove the swapdisc checks via "-rs" or "-ra".
	  this makes swapdisc checks always have the current disc inserted
	  and never start the swap process. this fixes some multidisc games
	  such as GTA5 and BF3.

v6.4
	* fixed import library handling.
	
	+ added "Xex Name" printing under Basefile Info heading

v6.3
	* fixed an issue where some xex files would not boot such as kinect xex files.
	
	* changed the special patching to list and let you select which patches to apply.
	  patches are done via bitflags so that multiple patches can be selected in one go.
	
	* changed the internal search and patch data for special patching of xam and xbdm
	  to support all known versions of these files.
