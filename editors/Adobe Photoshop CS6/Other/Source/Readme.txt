The base application's source code is available from the portable app's
homepage listed in the help.html file (if applicable).

Details of most other things are available there as well.

LICENSE
=======
This package's installer and launcher are released under the GPL. The launcher
is the PortableApps.com Launcher, available with full source and documentation
from http://portableapps.com/development. We request that developers using the
PortableApps.com Launcher please leave this directory intact and unchanged.

USER CONFIGURATION
==================
Some configuration in the PortableApps.com Launcher can be overridden 
by the user in an INI file next to PhotoshopPortable.exe called 
PhotoshopPortable.ini.

If you are happy with the default options, it is not necessary, though. 
There is an example INI included with this package to get you started. 
To use it, copy PhotoshopPortable.ini from this directory next to 
PhotoshopPortable.exe. The options in the INI file are as follows:

	AdditionalParameters=
	DisableSplashScreen=true
	AllowMultipleInstances=false
	VisualC++=true
	PSAutoRecover=true

(There is no need for an INI header in this file; if you have one, though, it
won't damage anything.)

The AdditionalParameters entry allows you to pass additional command-line
parameters to the application.

The DisableSplashScreen entry allows you to run the launcher without the splash
screen showing up. The default is true. To show again, simply set to false.

The AllowMultipleInstances entry allows you to run multiple instances of an
application that supports it. The default is false.

VisualC++ switch is for Windows XP users without Visual C++.
By default, this is set to `true`, which will provide support incase
Visual C++ is missing.

	To disable, simply set to false:
		ie. VisualC++=false

PSAutoRecover switch handles folders created by Photoshop used for storing
temporary files, recovery, caching, etc. This is a great feature except 
Photoshop does not always clean up after each session. 

When set to `true`, PhotoshopPortable will clean up this folder at exit.

	To disable, simply set to false: 
		ie. PSAutoRecover=false