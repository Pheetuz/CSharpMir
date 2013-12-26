CSharpMir
=========

C# LOM development

Ok folks,

This is the setup information for getting this all running - you will need visual studio 2012 installed to build and run these files - I am sure you can find a copy somewhere on the internet...

You will need to check out these files along with the other repository entitiles "ClientFiles".

Once these files have been checked out, go to CSharpMir\trunk\Legend of Mir.sln and open it - once it is open do a rebuild on release mode, then switch to debug mode - this will cause our output directories to be auto generated and save you the hassel.

Go to your CSharpMir directory, now in addition to the trunk folder you will have a Debug and a Release folder - these are our output directories for the build. 
Under Debug\Client, Release\Client, Debug\Server and Release\Server you will need to copy the Data, Map and Sounds directories and all of there contents (Yes, that is four locations that Data, Map and Sound need to be copied to - now you can see why it is a seperate check out at 1.45GB a pop).

Once this is done you are almost there, the next step depends on whether you are doing a debug or a release build - in the Debug\Server and Release\Server directories there is a file called Setup.ini, the top field in here is a version file path - set this to point to the Debug\Client\Client.exe file for a debug build and to Release\Client\Client.exe for a release build.

Once you have done this, do a full rebuild in VS and click play - this should get you in game.
