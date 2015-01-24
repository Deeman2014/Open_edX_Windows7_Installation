5. Starting & Stopping edX 
==========================

Background
^^^^^^^^^^

The edX platform will run under a virtual machine environment.

The platform runs under the Ubuntu operating system.

Once the platform has been installed, you can start it using VirtualBox.
 
|
Starting edX
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

5. Load the edX Learning Management System (LMS) by enter 192.168.33.10 into a browser on your Windows Host system.
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

Stopping edX
^^^^^^^^^^^^^^^^^

1. To log out of edX, CLICK the Staff or Student button at the top right of the Dashboard, and select Log Out.
     .. image:: ./_static/edX_logout.png

|  

2. To close the virtual machine, click the standard Close Window X icon at the top right of the window in which Ubuntu is running.
     .. image:: ./_static/Ubuntu_shutdown.png

|

3. Select the Power Off the machine, option and press CLICK the OK button. The window will close and the virtual machine will be unloaded.

