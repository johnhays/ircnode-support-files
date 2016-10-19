# ircnode-support-files
Support ircnodedashboard

Be sure you have an opendv user and group (which should have been created when ircddbgateway was installed)

**cd /etc/opendv**

**sudo wget https://raw.githubusercontent.com/johnhays/ircnode-support-files/master/etc/opendv/ircnodedashboard.conf**

**cd /etc/systemd/system**

**sudo wget https://raw.githubusercontent.com/johnhays/ircnode-support-files/master/etc/systemd/system/ircnodedashboard.service**

Make sure ircddbgateway is running or has previously been configured and run before starting the dashboard.

**sudo systemctl start ircnodedashboard**

**sudo systemctl enable ircnodedashboard**

