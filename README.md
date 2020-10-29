# ansible-spacewalk
Ansible project to setup spacewalk server and client sites

Spacewalk playbooks and roles
==============

      Two roles: Spacewalk-server-role and specewalk-client-role.

Spacewalk is an open-source package and system management solution for RedHat derivative distributions like CentOS, Scientific Linux and Fedora, developed by the spacewalk community.

 Spacewalk provides the web interface to manage and view the updates for the system that are registered with Spacewalk, and we can initiate the task such as install, update, inventory, and so on.


      Features

1. Inventory of the systems
2. Install and Update system packages.
3. Perform a Kick-start installation.
4. Deploy and Manage the configuration files from a single location
5. Start / Stop / Configure the guests.
6. Distribute the content across the multiple Geographical location using spacewalk proxy.



      Hardware and OS Requirements
      


1. Outbound open ports 80, 443
2. Inbound open ports 80, 443, 5222 (only if you want to push actions to client machines) and 5269 (only for push actions to a Spacewalk Proxy), 69 udp if you want to use tftp
3. Storage for the database: 250 KiB per client system + 500 KiB per channel + 230 KiB per package in a channel (i.e., 1.1GiB for a channel with 5000 packages)
4. Storage for packages (default /var/satellite): Depends on what you’re storing; Red Hat recommend 6GB per channel for their channels
5. 2 CPU , 4GB RAM minimum, 50GB disk minimum recommended

 