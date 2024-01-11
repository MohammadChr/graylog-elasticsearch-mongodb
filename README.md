![alt text](https://graylog.org/wp-content/uploads/2022/10/graylog-logo.svg)

graylog-installation-v1 :
 
With the help of this playbook, you can install Graylog, Elasticsearch, and MongoDB programs. 
This playbook is designed for a single-node cluster. It is written in a way that directly downloads and installs the programs on remote systems. 
For your convenience, a Vagrant file has been prepared in the following path (graylog-single-node) for quickly setting up an Ubuntu machine. 


graylog-installation-v2 :

This playbook is an optimized version of the previous one and is recommended for use in clusters with multiple nodes. 
In this version, files are downloaded once on the local system and then copied to the other nodes. 
A suitable Vagrant file for this approach is also provided in this path (3-node).
