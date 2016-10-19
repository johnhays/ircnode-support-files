# ircnode-support-files
Support ircnodedashboard

Be sure you have an opendv user and group (which should have been created when ircddbgateway was installed)

Place etc/opendv/ircnodedashboard.conf at /etc/opendv/ircnodedashboard.conf

Place etc/systemd/system/ircnodedashboard.service at /etc/systemd/system/ircnodedashboard.service

**sudo chown root:root /etc/opendv/ircnodedashboard.conf**

**sudo chmod 644 /etc/opendv/ircnodedashboard.conf**

**sudo chown root:root /etc/systemd/system/ircnodedashboard.service**

**sudo chmod 644 /etc/systemd/system/ircnodedashboard.service**

Make sure ircddbgateway is running or has previously been configured and run before starting the dashboard.

**sudo systemctl start ircnodedashboard**

**sudo systemctl enable ircnodedashboard**

