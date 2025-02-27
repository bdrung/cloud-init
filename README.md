# cloud-init

[![Build Status](https://travis-ci.com/canonical/cloud-init.svg?branch=main)](https://travis-ci.com/canonical/cloud-init) [![Read the Docs](https://readthedocs.org/projects/cloudinit/badge/?version=latest&style=flat)](https://cloudinit.readthedocs.org)

Cloud-init is the *industry standard* multi-distribution method for
cross-platform cloud instance initialization. It is supported across all
major public cloud providers, provisioning systems for private cloud
infrastructure, and bare-metal installations.

Cloud instances are initialized from a disk image and instance data:

- Cloud metadata
- User data (optional)
- Vendor data (optional)

Cloud-init will identify the cloud it is running on during boot, read any
provided metadata from the cloud and initialize the system accordingly. This
may involve setting up network and storage devices to configuring SSH
access key and many other aspects of a system. Later on cloud-init will
also parse and process any optional user or vendor data that was passed to the
instance.

## Getting help

If you need support, start with the [user documentation](https://cloudinit.readthedocs.io/en/latest/).

If you need additional help consider reaching out with one of the following options:

- Ask a question in the [``#cloud-init`` IRC channel on Libera](https://kiwiirc.com/nextclient/irc.libera.chat/cloud-init)
- Search the cloud-init [mailing list archive](https://lists.launchpad.net/cloud-init/)
- Better yet, join the [cloud-init mailing list](https://launchpad.net/~cloud-init) and participate
- Find a bug? [Report bugs on Launchpad](https://bugs.launchpad.net/cloud-init/+filebug)

## Distribution and cloud support

Below are a list of the many OSes and clouds that contain and ship with cloud-init. If your
distribution or cloud is not listed or does not have a recent version of cloud-init, please
get in contact with that distribution and send them our way!

| Supported OSes                                                                                                                                                                                                                                                                                                                                                                      | Supported Public Clouds | Supported Private Clouds |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------| --- | --- |
| Alpine Linux<br />Arch Linux<br />Container-Optimized OS<br />Debian<br />DragonFlyBSD<br />Fedora<br />FreeBSD<br />Gentoo Linux<br />NetBSD<br />OpenBSD<br />openEuler<br />OpenMandriva<br />RHEL/CentOS/AlmaLinux/Rocky/PhotonOS/Virtuozzo/EuroLinux/CloudLinux/MIRACLE LINUX/MarinerOS<br />SLES/openSUSE<br />Ubuntu<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /> | Amazon Web Services<br />Microsoft Azure<br />Google Cloud Platform<br />Oracle Cloud Infrastructure<br />Softlayer<br />Rackspace Public Cloud<br />IBM Cloud<br />DigitalOcean<br />Bigstep<br />Hetzner<br />Joyent<br />CloudSigma<br />Alibaba Cloud<br />Huawei Cloud<br />OVH<br />OpenNebula<br />Exoscale<br />Scaleway<br />CloudStack<br />AltCloud<br />SmartOS<br />HyperOne<br />Vultr<br />Rootbox<br /> | Bare metal installs<br />OpenStack<br />LXD<br />KVM<br />Metal-as-a-Service (MAAS)<br />VMware<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />|

## To start developing cloud-init

Checkout the [contributing](https://cloudinit.readthedocs.io/en/latest/development/contributing.html)
document that outlines the steps necessary to develop, test, and submit code.

## Daily builds

Daily builds are useful if you want to try the latest upstream code for the latest
features or to verify bug fixes.

For Ubuntu, see the [Daily PPAs](https://code.launchpad.net/~cloud-init-dev/+archive/ubuntu/daily)

For CentOS, see the [COPR build repos](https://copr.fedorainfracloud.org/coprs/g/cloud-init/cloud-init-dev/)

## Build / packaging

To see reference build/packaging implementations, refer to [packages](packages).
