Role Name
=========

A role installs vsftpd service on the managed host, creates folder /var/ftp/pub/upload, permits anonymous FTP read-access to /var/ftp/pub and upload to /var/ftp/pub/upload
vsftpd itself is configured as well to accept anonymous logins
The role opens firewall for FTP service and configures SELinux for anonymous FTP and to allow upload to /var/ftp/pub/upload

Role Variables
--------------

Variables in vars directory are used for template that creates vsftpd.conf file with required parameteres from the scratch. Parameters related to anonymous login are defined as variables there.

Author Information
------------------

https://github.com/Iurii-B/devops-school-ansible
