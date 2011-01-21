JBKinectHacks
=============
By John Boiles
http://github.com/johnboiles/JBKinectHacks

A collection of sample projects and code snippets using OpenNI and the Kinect.
Only tested on OSX.

To build using the included makefiles, libOpenNI.dylib must be
installed in /usr/lib and the OpenNI includes must be in /usr/include/ni.

To build using the xcode project, you must symlink /usr/include/ni and
/usr/lib/libOpenNI.dylib to the appropriate places in your developer install.
AFAIK there's not an elegant way to get xcode to use the standard /usr/include
and /usr/lib paths. For my installation I ran the following commands:

<pre>sudo ln -s /usr/lib/libOpenNI.dylib /Developer/SDKs/MacOSX10.6.sdk/usr/lib/libOpenNI.dylib</pre>

<pre>sudo ln -s /usr/include/ni /Developer/SDKs/MacOSX10.6.sdk/usr/include/ni</pre>

Note that the binaries expect a file named SamplesConfig.xml to be in the present working
directory when they are run.

To Install OpenNI for Mac
-------------------------
1.   Get OpenNI

<pre>git clone git://github.com/OpenNI/OpenNI.git</pre>

2.   Switch to unstable branch (only unstable supports osx atm)

<pre>git checkout unstable</pre>

3.   Follow the installation instructions in the Readme (they're pretty good)

4.   Get the unstable forked version of the PrimeSense/Sensor module working

<pre>git clone git://github.com/ros-pkg-git/Sensor.git</pre>

5.   Follow the installation instructions in the Readme (they're also pretty good)

6.   Get the PrimeSense NITE binaries here:
http://www.openni.org/component/search/?searchword=nite&ordering=&searchphrase=all

7.   Run the install script included with the NITE binaries

<pre>sudo ./install.sh</pre>

8.   Use License code

<pre>0KOIk2JeIBYClPWVnMoRKn5cdY4=</pre>