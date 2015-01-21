Prerequisites
=============
This section describes the prerequisites for installing Open edX.

The Required Software Prerequisites
-----------------------------------

The Open edX platform has been implemented using a wide variety of software, including the python, ruby, and django programming languages, MySQL and mongodb database systems, the Nginx web server package, and the postfix email management system, to name a few.

To help ensure that the necessary software has been properly installed and configured to work together, several software installation and provision packages have been utilized.

To reduce the likelihood that the resulting edX development environment software will interfere with, or be disturbed by, other software already running on your computer, a virtual environment is used.
The virtual environment created allows you to install an additional operating system, where you can then install all the software, and run the operating system and any software installed on it alongside your original operating system.

In our case, we will use Microsoft Windows 7 Enterprise as the host operating system. On that operating system we must install a few software packages, after which we can then use scripts provided by Open edX and supporters to install the rest of the edX platform code.

You will need the following software:
 #. Windows Enterprise 7 64
 #. Virtual Box 4.3.16r95972
 #. Vagrant 1.5.4
 #. curl 
 
It would be wise to go ahead and install these packages as our first step.

| 
1. Windows 7 Enterprise
--------------------

First, you will need the host operating system, Windows Enterprise 7.

A license for Microsoft Windows 7 Enterprise must be acquired separately.

You need the Enterprise (or Ultimate) version because that version comes with a package that you will need, called Network File Sharing Client Servies for Unit (NFS).

Windows 7 Professional and other versions of Windows 7 do not come with the package.

You can buy a copy of Windows 7 Enterprise from Microft, a retail store, or online.

You can also download a copy of it from Microsoft here: 

#. http://www.microsoft.com/en-us/evalcenter/evaluate-windows-7-enterprise

| 
2. Oracle VirtualBox
-----------------

Oracle VirtualBox is an open source (free) software package that will allow you to install additional operating systems onto your computer that will run from within Windows 7.

VirtualBox will give you the ability to create a *virtual machine*, which is a separate operating system environment into which you can install software and save data files.

The homepage for Oracle VirtualBox is here: https://www.virtualbox.org/

You need to download Oracle VirtualBox, and the companion extension pack for it.

You can find the versions you need for 64-bit Windows 7 here:

#. VirtualBox 4.3.16 - http://download.virtualbox.org/virtualbox/4.3.16/VirtualBox-4.3.16-95972-Win.exe 
#. VirtualBox 4.3.16 Extension Pack - http://download.virtualbox.org/virtualbox/4.3.16/Oracle_VM_Virtualx_Extension_Pack-4.3.16-95972.vbox-extpack

| 

3. Vagrant
----------

Vagrant is an open source (free) software package that will allow you to run scripts to more easily and reliably install and configure software.

It is very useful for installing simple and complex software environments.

Vagrants scrips have been developed to install Open edX. Using these scripts will allow you to install the bulk of the operating environment for Open edX.

The homepage for Vagrant is here: https://www.vagrantup.com/

The Vagrant version we will use is 1.5.4.

You can find the Vagrant Version 1.5.4 that you need for 64-bit Windows here:

#. Vagrant 1.5.4 - https://dl.bintray.com/mitchellh/vagrant/vagrant_1.5.4.msi 

| 

4. curl
-------

curl is open source (free) software that will allow you to download software.

curl is a command line tool and library for transferring data with URL syntax

This software will be used to download the Vagrant script file that you will use to install the edX environment.

The homepage for Cygwin is here: http://www.cygwin.com/

You can find the curl version that you need for 64-bit Windows here:

#. curl - http://cygwin.com/setup-x86_64.exe 


