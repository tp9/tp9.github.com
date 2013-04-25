---
layout: post
title: "Installing Pygame"
description: ""
category: 
tags: [pygame, step-by-step]
---
{% include JB/setup %}
_Step 1: Download python 2.7_  
The first thing you need to do is download and install your Python environment.
I'm currently on 2.7 so if you plan on following the tutorials on this blog
you'll need 2.7.  
[Windows](http://www.python.org/ftp/python/2.7.4/python-2.7.4.msi)  
[Windows 64](http://www.python.org/ftp/python/2.7.4/python-2.7.4.amd64.msi)  

_Step 2: Install python_  
Once you've completed your download, launch the msi file and follow the prompts.
The installer should install to C:\Python27.  
  
Once the install is completed you want to make sure your path variable is set in
Windows. Go to System Properties -> Environment Variables and under System
variables select Path and click the Edit button. This will bring up the Edit
System Variable window. In Variable value, go to the beginning of the path string
and make sure "C:\Python27;" is there, if not you can add it in and click OK.  
  
Finally, open a command prompt and type in "python" at the prompt. You should
see the version information and a python prompt loaded. Type "exit()" to get back
to your Windows prompt and close the command window.  

_Step 3: Download pygame_  
Now you need to download and install the Pygame library. NOTE: The 64-bit version
is a pre-release version but that's the version I'm on and I haven't run into any
problems yet.  
[Windows](http://pygame.org/ftp/pygame-1.9.2a0.win32-py2.7.msi)  
[Windows 64](http://www.lfd.uci.edu/~gohlke/pythonlibs/#pygame)  

_Step 4: Install pygame_  
Once you've completed your download, launch the executable and follow the prompts.
The install program should locate your Python 2.7 installation in "C:\Python27".
Just continue with the defaults and the installer will place the Pygame library
in your Python folder under "C:\Python27\include\pygame".  
  
And you're done. If you want to test the installation you can go back to your
command prompt and type in "python" then "import pygame". If the installation
was successful you shouldn't see an error. Welcome to Pygame development!  
