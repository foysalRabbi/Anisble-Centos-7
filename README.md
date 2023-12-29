# LAMP_Ansible_Centos7

The term "LAMP_Ansible_Centos7" seems to refer to a specific technology stack and configuration used in IT and software development. Let's break down the components:
# LAMP:

1. L: Stands for Linux, the operating system.
2. A: Stands for Apache, the web server.
3. M: Stands for MySQL or MariaDB, the relational database management system.
4. P: Stands for PHP
   
LAMP is a popular open-source web development stack used for building dynamic web applications and websites.

# Ansible:

Ansible is an open-source automation tool that is used for configuration management, application deployment, task automation, and orchestration. It simplifies complex tasks, making it easier to manage and scale infrastructure.
CentOS 7:

CentOS is a free and open-source Linux distribution based on the sources of Red Hat Enterprise Linux (RHEL). CentOS 7 is a specific version of CentOS.

# Note: Don't change any directory Name. and clone this project to your root directory.
This repository is only for practice purpose.

This repository will work on centos 7 for LAMP Stack (Apache, PHP8.1, Mariadb)
This is a php base web application backed with mysql Database.
In you ansible Host file locatted /etc/ansible/hosts or you can configure your custome inventory file for this stack. In your invantory file server group name should be as following:

Ansible Inventory Configuration:

[web] for web server configuration. you just configure your server ip under this group for web configuration.

[ha] for HAProxy confguraiton group name. you just place your HAProxy server ip under this group.

[db] for Database group name. place you DB server ip under this group.

Change in sample code:

In config.php file replace your database ip address here. File location: code/config.php

In HAProxy configuration file just change your webserver ip address. File location: cfg/haproxy.cfg



All done now just run yml file as per secquence or you can run all_task.yaml

1. repository_installation.yml
2. apache-with-php.yml
3. mariadb-installation.yml
4. mysql-user-mgmt.yml
5. haproxy-installation.yml

lets browse from your website link: http://your_haproxy_ip/code
It will open a php site.
