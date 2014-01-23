SCHIZOID for HP Touchpad (tenderloin)
============================================

Getting Started
---------------

To get started with SCHIZOID, you'll need to get
familiar with [Git and Repo](http://source.android.com/download/using-repo).

To initialize your local repository using the Schizoid Tenderloin trees, use this command:

    repo init -u git://github.com/shumashv1/Schizoid.git -b cm-10.1

Then to sync up (Schizoid defaults to -j16, so set it to something else if you want):

    repo sync
The inital sync takes as much time to complete as a build, so expect to wait a LONG time to complete.

To build, make sure you're in your build directory, i.e. ~/android/skz, or whatever, then type in the terminal window

    . build/envsetup.sh (note the space between . and build)

When that completes, type "lunch" and select the number corresponding to "skz_tenderloin-userdebug"

Type "make bacon", wait a another LONG time while it compiles and builds.

You will find your installation skz_(something).zip file waiting in the out/target/product/tenderloin
directory or you can just type "cd OUT$"
