1. Microsoft Windows 7 Enterprise
=================================

Windows 7 Enterprise will be the base operating system onto which all the other software will be installed.

We will refer to it as the *host* operating system.

You need the Enterprise (or Ultimate) version because that version comes with a systems service that the edX platform needs, called Client for Network File Ssystem (NFS).

Windows 7 Professional, and other versions of Windows 7, do not come with this NFS service.

You can buy a copy of Windows 7 Enterprise from Microsoft, a retail store, or online.

You can also download a 90 day evaluation copy of it from Microsoft here: 

#. http://www.microsoft.com/en-us/evalcenter/evaluate-windows-7-enterprise


Installing Windows 7 Enterprise and Enabling Network File System (NFS)
----------------------------------------------------------------------

Install Windows 7 Enterprise as normal.

After installing it, ensure that the Client for Network File System (NFS) service has been enabled.

We can use the Windows 7 msconfig.exe program to enable it.

To enable Client for NFS, you can use the following steps:

1. Click the Start button at the bottom left of the Windows Start menu. Then type msconfig into the text box just above the menu bar:
     .. image:: ./_static/msconfig_1.jpg

|
2. msconfig.exe will display at the top of the Search results. Click it to launch the msconfig.exe program.
     .. image:: ./_static/msconfig_2.jpg

|
3. Once the dialog box displays, click the Services tab.
     .. image:: ./_static/msconfig_3.jpg

|
4. Scroll through the list until you locate Client for NFS
     .. image:: ./_static/msconfig_4.jpg

|
5. Once found, ensure that it is checked. 
     .. image:: ./_static/msconfig_5.jpg

|
That completes the process for enabling the Client for NFS service.

That is the only initial Windows 7 Enterprise configuration needed for the Open edX platform.

