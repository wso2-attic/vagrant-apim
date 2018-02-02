# Vagrantfile for WSO2 API Manager

This section defines the procedure to execute run Vagrant resources for a setup of WSO2 API Manager single
node with Analytics support.

![Deployment architecture](deployment-diagram.png)

Please note that in order to run these Vagrant resources use, you need to install
[Oracle VM VirtualBox](http://www.oracle.com/technetwork/server-storage/virtualbox/downloads/index.html),
as Vagrant uses Oracle VM VirtualBox as the default provider.

Virtualization should be enabled in BIOS settings before building the boxes.

## How to run the Vagrantfile

1. Checkout this repository into your local machine using the following Git command.

```
    https://github.com/wso2/vagrant-apim.git
```

2. Build Vagrant boxes for external MySQL database, WSO2 API Manager and API Manager Analytics using the Vagrant box automation resources.

3. Move to `vagrantfiles` folder.

```
    cd vagrantfiles
```
4. Spawn up the Vagrant setup.

```
    vagrant up
```
