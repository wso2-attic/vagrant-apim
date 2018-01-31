# Vagrant box generation

This section defines the procedure to build Vagrant boxes required for WSO2 API Manager 2.1.0

Please note that in order to build these Vagrant boxes, you need to install
[Oracle VM VirtualBox](http://www.oracle.com/technetwork/server-storage/virtualbox/downloads/index.html),
as WSO2 Vagrant resources use Oracle VM VirtualBox, as the default provider.

Virtualization should be enabled in the BIOS before building the boxes.
## How to build the Vagrant boxes


### Vagrant box build process


1. Checkout this repository into your local machine using the following Git command.
```
	git clone https://github.com/wso2/vagrant-apim.git
```

2. Download
	[WSO2 API Manager 2.1.0](https://wso2.com/api-management/#download), [JDK 8u144-linux-x64.tar](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html), [MySQL Connector/J](https://dev.mysql.com/downloads/connector/j/) and [WSO2 Update Manager](https://wso2.com/wum/download). Copy them to the following path. 

Note: Adding WSO2 Update Manager is optional. Read more about [WSO2 Update Manager](https://wso2.com/wum/).
```
	~/vagrantboxes/files/
```
3. Move to `boxes` folder.
```
	cd boxes
```
4. Execute the build.sh shell script.
```
	./build.sh
```
5. Add created box files to local Vagrant box cache.

The created box files can be found in the output directory. In order to add a created box to the local Vagrant box cache use the `vagrant box add` command.

```
	vagrant box add <BOX_NAME> <BOX_FILE_PATH>
```

An example for adding the created WSO2 API Manager Vagrant box file (by default, defined
within the `config.yaml` file) is as follows:

```
	vagrant box add wso2am output/wso2am.box
```


