7. Install edX 
==============

Background
^^^^^^^^^^

The edX platform is based an a wide variety of software components.

Each component must be of the right (compatible) version, and must be configured to work well with the other components.

To help ensure that all the software has been installed and configured as required, installation, provisioning, and configuration software from Vagrant and Ansible has been used.

A script written in the Vagrant scripting language will be used, which will call other pograms, including Ansible scripts.

This makes it possible for a person to install the base edX platform with just a few commands.

|
Prerequisites
^^^^^^^^^^^^^

To install Open edX using the Vagrant script, the following software must have already been installed:

1. Windows 7 Enterprise, with Services for NFS enabled.
2. Oracle VirtualBox 4.3.16 and its extension pack.
3. Vagrant 1.5.4
4. cURL version 7.40.0

|
Installing the edX Platform
^^^^^^^^^^^^^^^^^^^^^^^^^^^

The edX Platform is packaged in a VirtualBox image or "box". 

For the purposes of these instructions, we will install the birch release of edX. 

The size of the box for the birch release is approximately 2.8GB. It will take a while to download.

The Vagrant installation script will download the box, create a VirtualBox virtual machine instance with Ubuntu as the operating system, and then install and configure all the code it needs into Ubuntu within that virtual machine.

We will install the edX Platform by running the Vagrant script from the command line.

All you have to do is create the directory from which you would like to run edX, and run the Vagrant script.

So, let "edx_birch" will be the name of the directory. You can, however, use any name you like.


1. Open a command line session with Administrator Rights, by Clicking the Start Button, Accessories, and Command Prompt. 
     Right click it, and select Run as Administrator.

     .. image:: ./_static/commandline.png

|
2. Create a directory for edX: 
      md \edx_birch

|
3. Make that directory the current directory: 
      cd \edx_birch

|
4. Download the Vagrant script file, using the cURL programs, by copy and pasting curl line below into the command prompt window, and pressing ENTER. (You can use the mouse to copy the following line. You will have to use the mouse to also paste it into the command line window. You cannot use CTRL C followed by CTRL V.)
    curl -L https://raw.githubusercontent.com/edx/configuration/master/vagrant/release/fullstack/Vagrantfile > Vagrantfile

   Note: The Vagrantfile you will download with the previous command will default to installing the kifli version of edX, not the birch version.

   To install the birch release:

   1. Create an *OPENEDX_RELEASE* environment variable in Windows
       * Create the Windows environment variable: OPENEDX_RELEASE="named-release/birch"
       
       To do so:
          1. Click the Start button, right click My Computer and select Properties.
          2. Click the Advanced Systems Settings option on the panel on the left.
          3. Click the Environment Variables button.
          4. In the System Variables List, at the bottom half of the window, click the New... button.
          5. Enter as the Variable Name: OPENEDX_RELEASE
          6. Enter as the Variable Value: named-release/birch
          7. Click OK to save the new system variable.
          8. Reboot the computer immediately.
   

   2. Modify the newly downloaded Vagrantfile, replacing the default reference with a reference to the named-release/birch version.
   
|
5. Install the Vagrant hostsupdater plugin:
      vagrant plugin install vagrant-hostsupdater

|
6. Create the Fullstack virtual machine, by having Vagrant run the script:
      vagrant up

|
7.  Reboot the computer.
      
