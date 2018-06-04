# PythonAppLauncher
C++ code for a python application launcher on Windows in order to ease packaging
process

## Summary

C++ code to create an executable file to launch python applications with the
following goals:

- dynamically load Python DLL
 - allows to have the executable outside the main python directory, but still
   set the python runtime and ignore system python settings
- overwrite PYTHONPATH to ignore system Python settings
- set PYTHONHOME in order to specify a packaged python runtime
- accept command line arguments and pass to python application

## Using This Code

Use this code to write your own application launcher
Currently uses Microsoft Visual C++.  The build.bat sets up the environment to
use the MSVC Build Tools and compile with the appropriate options from the
command line

Change 'App' to whatever your application name is, provide a .ico file or just
disable the linking in the .bat file.
