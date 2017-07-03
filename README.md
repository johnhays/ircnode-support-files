# ircnode-support-files
Support ircnodedashboard

Be sure you have an opendv user and group (which should have been created when ircddbgateway was installed)

**cd /etc/opendv**

**sudo wget https://raw.githubusercontent.com/johnhays/ircnode-support-files/master/etc/opendv/ircnodedashboard.conf**

**cd /etc/systemd/system**

**sudo wget https://raw.githubusercontent.com/johnhays/ircnode-support-files/master/etc/systemd/system/ircnodedashboard.service**

This service file looks for node in /usr/local/bin -- edit it if yours is at another location.

Make sure ircddbgateway is running or has previously been configured and run before starting the dashboard.

**sudo systemctl start ircnodedashboard**

**sudo systemctl enable ircnodedashboard**

The dashboard should be available on the local machine at http://localhost or over the LAN at the machine's IP address.  If you need to change the port from 80 or limit it to a specific IP interface, edit webserver.js
