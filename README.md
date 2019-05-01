# Kivy and Buildozer Installer

The kivy_buildozer_installer.sh is automating my actions I have shown in this [video](https://www.youtube.com/watch?v=IzKJgpJrrQU).

The complete list of Buildozer dependencies is:

-    build-essential
-    ccache
-    git
-    libncurses5:i386
-    libstdc++6:i386
-    libgtk2.0-0:i386
-    libpangox-1.0-0:i386
-    libpangoxft-1.0-0:i386
-    libidn11:i386
-    python2.7
-    python2.7-dev
-    openjdk-8-jdk
-    unzip
-    zlib1g-dev
-    zlib1g:i386
-    **libltdl-dev**
-    **libffi-dev**
-    **libssl-dev**
-    **autoconf**
-    **autotools-dev**
-    cmake


## Installation Kivy and Buildozer on Ubuntu 18.04 based distros

The kivy-buildozer-installer.sh installs Kivy framework and Buildozer for Python 3 with all its dependecies.

The script was successfully tested with Xubuntu 18.04 and Lubuntu 18.04. The test result was a successfully compiled .apk file for Android 6.0 and 7.0.

1. Download the [**kivy-buildozer-installer.sh**](https://raw.githubusercontent.com/zaemiel/kivy-buildozer-installer/master/kivy-buildozer-installer.sh?token=AB6EA2GUYKRGLNKO4COJQNS4ZG3QE) any way you like. E.g.

    ```curl -LJO https://raw.githubusercontent.com/zaemiel/kivy-buildozer-installer/master/kivy-buildozer-installer.sh?token=AB6EA2GUYKRGLNKO4COJQNS4ZG3QE```

2. Add execution permissions:

    ```chmod +x kivy-buildozer-installer.sh```

3. Run the script:

    ```sudo ./kivy-buildozer-installer.sh```


WARNING.
With manual installation of the Buildozer via cloning its repository, pay attention to clone the Buildozer repository to any directory except HOME directory. Otherwise the error "**AttributeError 'Namespace' object has no attribute 'ignore-setup_py'**" will occur probably due importing modules conflicts.

____________

## Buildozer Virtual Machine

The current virtual machine allow
you to have a ready to use VM for building Android application.

### Download Buildozer VirtualBox Machine:

Lubuntu 18.04 Virtual machine (Unziped size is about **13 Gb**):

1. [Yandex.Disk - 4.9 Gb](https://yadi.sk/d/P8Vw_2xXLJKNCA)




### Using shared folders

1. Create a folder on your host machine.

2. In the Virtualbox menu: 'Devices' -> 'Shared folders' -> 'Shared folders settings...' click on the small button at the right side 'Adds new shared folder'

3. Specify the folder path on your host machine

4. Check 'Auto-mount' and 'Make permanent' boxes.

5. Power off your guest machine

6. Start the guest machine again and shared folder should appear on the Desktop.

7. Done


#### If Android dependencies are outdated execute:

```buildozer android update```
