Project: jexbackup
Author: Denis Shapovalov
Email: 

Based on: https://pypi.python.org/pypi/esbackup/0.2 by Alexander Samarin

Installation:
 1. Copy from ${PREFIX}/lib/python2.7/site-packages/esbackup/sample/esbackup_config.py to
    /etc/esbackup_config.py (or /usr/local/etc/esbackup_config.py depending on your system).
    Configure it for your needs.
 2. Add to the /etc/crontab file (change the line to conform your OS):
     10 2 * * * root /usr/local/bin/python2.7 -m esbackup.cron > /var/log/esbackup.log 2>&1
