7. Install edX 
==============

Background
^^^^^^^^^^

The edX platform is based an a wide variety of software components.

Each component must be of the right (compatible) version, and must be configured to work with the others well.

To help ensure that all the software has been installed and configured as required, installation and provision software from Vagrant and Ansible have been used.

A script written using the Vagrant scripting language has been used, which calls other pograms, including Ansible scripts.

This makes it possible for a person to install the base edX platform with just a few commands.

|
Prerequisites
^^^^^^^^^^^^^

To install Open edX using the Vagrant script, you must have already installed the following software:

1. Windows 7 Enterprise, with Services for NFS enabled.
2. Oracle VirtualBox 4.3.16 and its extension pack.
3. Vagrant 1.5.4
4. cURL version 7.40.0

|
Installing the edX Platform
^^^^^^^^^^^^^^^^^^^^^^^^^^^

The edX Platform is packaged in a VirtualBox image, or box. The box for the edX Aspen.1 release is 2.78GB.

So, it will take a while to download.

The Vagrant installation script will download the box, create a VirtualBox virtual machine instance with Ubuntu as the operating system, and then install and configure all the code it needs into Ubuntu within that virtual machine.

We will install the edX Platform manually by running the Vagrant script from the command line.

All you have to do is create the directory from which you would like to run edX, and run the script, as follows.



 1.  Open a command line session with Administrator Rights, by Clicking the Start Button, Accessories, and Command Prompt. 
        Right click it, and select Run as Administrator.

     .. image:: ./_static/commandline.png


 2. Create a directory for edX: 
      md \edx_aspen


 3. Make that directory the current directory: 
      cd \edx_aspen


 4. Download the Aspen.1 fullstack Vagrant script file, using the cURL programs, by copy and pasting this line into the command prompt window, and pressing RETURN:
      curl -L https://raw.githubusercontent.com/edx/configuration/master/vagrant/release/fullstack/Vagrantfile > Vagrantfile


 5. Install the Vagrant hostsupdater plugin:
      vagrant plugin install vagrant-hostsupdater


 6. Create the Fullstack virtual machine, by having Vagrant run the script:
      vagrant up

 7.  Reboot the computer.
  

|
Running edX
^^^^^^^^^^^

  1. Load the VirtualBox program by clicking it on the Start Menu or double clicking its program icon.
      .. image:: ./_static/VirtualBox_icon.png


  2. Click the Aspen entry on the lefthand side of the VirtualBox interface, and then click Start from the menu above.
     
     .. image:: ./_static/Virtual_Box_4.3.16_edX.png

|

  3. The virtual machine will start in a command window. Some commands will be run in that window. Wait for them to complete.
  
     .. image:: ./_static/virtual_machine_start.png

|

  4. After the login screen has loaded, wait another 10-15 seconds to allow any background proccesses to complete.
  
     .. image:: ./_static/Ubuntu_running.png


     edX is already loaded at this point. You do not have to login. 
|

  6. Load the edX Learning Management System (LMS) by enter 192.168.33.10 into a browser on your Windows Host system.
      If the installation went went well, the LMS will load and display a welcome the initial Welcome page.
  
     .. image:: ./_static/edX_LMS.png

|

  6. Load Studio, the edX Content Management System (CMS), by entering 192.168.33.10:18010 into a browser:
      
     .. image:: ./_static/edX_CMS.png

|

  7. Login using a pre-built user account: ID: staff@example.com  Password: edx

     .. image:: ./_static/edX_login.png

|

  8. You are now logged into edX and your Dashboard of registered courses is display.

     .. image:: ./_static/edX_logged_in.png

|  

  9. To log out of edX, CLICK the Staff or Student button at the top right of the Dashboard, and select Log Out.

     .. image:: ./_static/edx_logout.png

|  

  10. To close the virtual machine, click the standard Close Window X icon at the top right of the window in which Ubuntu is running.

      .. image:: ./_static/Ubuntu_shutdown.png

|

  11. Select the Power Off the machine, option and press CLICK the OK button. The window will close and the virtual machine will be unloaded.

