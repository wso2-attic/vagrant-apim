# Vagrantfile for WSO2 API Manager


This section defines the procedure to run Vagrant resources for a setup of WSO2 API Manager single
node with Analytics support.

![Deployment architecture](deployment-diagram.png)

Please note that in order to run these Vagrant resources use, you need to install
[Oracle VM VirtualBox](http://www.oracle.com/technetwork/server-storage/virtualbox/downloads/index.html),
as Vagrant uses Oracle VM VirtualBox as the default provider.

Virtualization should be enabled in BIOS settings before building the boxes.

## How to run the Vagrantfile

1. Build the WSO2 API Manager 2.1.0, WSO2 API Manager Analytics 2.1.0, and MySQL boxes by following the instructions given in https://github.com/wso2/vagrant-boxes

2. Checkout this repository into your local machine using the following Git command.

```
    https://github.com/wso2/vagrant-apim.git
```

3. Move to `vagrant-apim` folder.

```
    cd vagrant-apim
```
4. Spawn up the Vagrant setup.

```
    vagrant up
```

5. Access the API Publisher and Store via the URLs given below.

* API Publisher

```
    https://172.28.128.4:9443/publisher/
```

* API Store

```
    https://172.28.128.4:9443/store/
```

* Carbon

```
    https://172.28.128.4:9443/carbon/
```

* Admin

```
    https://172.28.128.4:9443/admin/
```
