# Vagrantfile for WSO2 Identity Server

This section defines the procedure to execute run Vagrant resources for a setup of WSO2 API Manager single
node with Analytics support.

Please note that in order to run these Vagrant resources use, you need to install
[Oracle VM VirtualBox](http://www.oracle.com/technetwork/server-storage/virtualbox/downloads/index.html),
as Vagrant uses Oracle VM VirtualBox as the default provider.

Virtualization should be enabled in BIOS settings before building the boxes.
## How to run the Vagrantfile

##### 1. Checkout this repository into your local machine using the following Git command.
```
git clone https://github.com/wso2/vagrant-apim
```

##### 2. Build Vagrant boxes for external MySQL database, WSO2 API Manager and API Manager Analytics using the Vagrant box automation resources.

##### 3. Move to `machines` folder.

    cd machines

##### 4. Spawn up the Vagrant setup.

    vagrant up
