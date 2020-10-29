     Role Name
=========

Spacewalk-client-role
=========

A brief description of the role goes here.
Requirements

------------
The Spacewalk client packages have dependencies in the EPEL repositories. Install those:
# yum install epel-release -y
Next, install the EL7 Spacewalk client repository:
# rpm -Uvh https://copr-be.cloud.fedoraproject.org/results/%40spacewalkproject/spacewalk-2.10-client/epel-7-x86_64/01258160-spacewalk-repo/spacewalk-client-repo-2.10-8.el7.noarch.rpm
Finally, install the required client packages:
# sudo yum install rhn-client-tools rhn-check rhn-setup rhnsd m2crypto yum-rhn-plugin
Register the Spacewalk Clients
# rhnreg_ks --serverUrl=http://3.237.15.210/XMLRPC --activationkey=1-8be4b4528480688e6d4eda693a792c4c

