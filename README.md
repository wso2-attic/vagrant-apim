# WSO2 API Manager Vagrant
Vagrant is an open-source software product for building and maintaining portable virtual software development environments, e.g. for VirtualBox, Hyper-V, Docker, VMware, and AWS. The core idea behind it lies in the fact that the environment maintenance of virtualizations becomes increasingly difficult in a large software development project. Vagrant simplifies the necessary software configuration management in order to increase development productivity. Vagrant is written in the Ruby language, but its ecosystem supports development in almost all major languages.

## Boxes
This contains the source code of obtaining 3 ubuntu/trusty64 vboxes as the base boxes and adding the WSO2 API Manager, WSO2 API Manger-Analytics and MYSQL to each box with the relevant JDK version. The WSO2 Server files are extracted inside each vbox. These boxes are automatically added to to the local Vagrant box cache.

## Vagrantfile
The 3 vboxes added previously to the local Vagrant box cache are configured with the necessary IPs and Ports. Also the WSO2 API Manager Server is deployed inside the vbox and could be evaluated by logging into the management console through the web browser.
