# Vagrantfile for WSO2 API Manager

In order to use Vagrant boxes with updates, you will need an active subscription from WSO2 since the Vagrant boxes hosted at vagrant.wso2.com contains the latest updates and fixes to WSO2 API Manager. You can sign up for a Free Trial Subscription [here](https://wso2.com/free-trial-subscription).

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
   > If you are to try out an already released zip of this repo, please ignore this 1st step.


2. Move to `vagrant-apim` folder.

```
cd vagrant-apim
```
>If you are to try out an already released zip of this repo, please ignore this 2nd step also. Instead, extract the zip file and directly browse to `vagrant-apim-<released-version>` folder.

>If you are to try out an already released tag, after executing 2nd step, checkout the relevant tag, i.e. for example: <br> git checkout tags/v3.0.0.1 and continue below steps.

3. Switch to WSO2 API Manager deployment pattern directory

```
cd < deployment-pattern-directory >
```

4. Spawn up the Vagrant setup.

```
vagrant --updates up
```

If you wish to use the Vagrant boxes without updates, spawn up the Vagrant setup as follows.

```
vagrant up
```
