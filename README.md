# Vagrantfile for WSO2 API Manager

In order to use Vagrant boxes, you will need an active subscription from WSO2 since the Vagrant boxes hosted at vagrant.wso2.com contains the latest updates and fixes to WSO2 API Manager. You can sign up for a Free Trial Subscription [here](https://wso2.com/free-trial-subscription).

If you wish to use the Vagrant boxes without updates, please build them from [here](https://github.com/wso2/vagrant-boxes).

This section defines the procedure to run Vagrant resources for a setup of WSO2 API Manager single
node with Analytics support.

Please note that in order to run these Vagrant resources use, you need to install
[Oracle VM VirtualBox](http://www.oracle.com/technetwork/server-storage/virtualbox/downloads/index.html),
as Vagrant uses Oracle VM VirtualBox as the default provider.

Virtualization should be enabled in BIOS settings before building the boxes.

## How to run the Vagrantfile

1. Checkout this repository into your local machine using the following Git command.

```
    https://github.com/wso2/vagrant-apim.git
```

2. Move to `vagrant-apim` folder.

```
    cd vagrant-apim
```

3. Switch to WSO2 API Manager deployment pattern directory

```
    cd < deployment-pattern-directory >
```

4. Spawn up the Vagrant setup.

```
    vagrant up
```
