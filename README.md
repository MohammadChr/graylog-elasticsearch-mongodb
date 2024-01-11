![alt text](https://graylog.org/wp-content/uploads/2022/10/graylog-logo.svg)

graylog-installation-v1 :
 
With the help of this playbook, you can install Graylog, Elasticsearch, and MongoDB programs. 
This playbook is designed for a single-node cluster. It is written in a way that directly downloads and installs the programs on remote systems. 
For your convenience, a Vagrant file has been prepared in the following path (graylog-single-node) for quickly setting up an Ubuntu machine. 


graylog-installation-v2 :

This playbook is an optimized version of the previous one and is recommended for use in clusters with multiple nodes. 
In this version, files are downloaded once on the local system and then copied to the other nodes. 
A suitable Vagrant file for this approach is also provided in this path (3-node).

NOTICE:

#Please make sure to change the :
- hosts: graylog
to appropriate names before using.

#This line is used to address sanctions-related issues. If you are using a proxy or not under sanctions , you can comment out this line
    - name: DNS
      lineinfile:
        path: /etc/resolv.conf
        line: 'nameserver 178.22.122.100'
        state: present

#

Currently, this playbook only handles the download and installation process. I am working to quickly incorporate the cluster setup process into it as well.

