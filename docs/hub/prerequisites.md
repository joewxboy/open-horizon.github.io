---
copyright: Contributors to the Open Horizon project
years: 2021 - 2026
title: Prerequisites for full installation
description: Documentation for Install {{site.data.keyword.ieam}}
lastupdated: 2026-08-20
nav_order: 1
parent: Installing Open Horizon
---

{:new_window: target="blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}
{:child: .link .ulchildlink}
{:childlinks: .ullinks}

# Install {{site.data.keyword.ieam}}
{: #hub_install_overview}

You must install and configure a management hub before you start the {{site.data.keyword.edge_notm}} node tasks.

## Prerequisites for full installation
{: #prereq}

* Ensure you are using a Debian-based {{site.data.keyword.linux}} distribution such as Ubuntu 20.04 or 22.04 LTS and running on an x86-based micro-architecture. The installation can run on the bare hardware or in a VM.  The Hub **cannot** run on arm64-based hardware.
* For installation, you will need to become root, ex. `sudo -i`
* Ensure that you know the public or network facing IP address for the local network that other machines will use to connect to the Management Hub. We will set that IP address as `HZN_LISTEN_IP`. If you do not set this in advance, other machines will not be able to connect to the hub.
* {{site.data.keyword.edge_notm}} uses Mongo 6. If you want to run {{site.data.keyword.edge_notm}} using only open source tools, you must set a variable to override the version of Mongo. Set the `MONGO_IMAGE_TAG` environment variable to 4.0.6.
* If you are using Podman or any container engine that is not Docker, you must set the `DOCKER_ENGINE` variable appropriately. For example, if you are using Podman, run this command: 
  ```shell
  export DOCKER_ENGINE=podman
  ```

## Gathering edge node files

Several files are needed to install the {{site.data.keyword.edge_notm}} agent on your edge devices and edge clusters and register them with {{site.data.keyword.edge_notm}}. These agent files are stored in the CSS Cloud Sync Service (CSS) component of the Model Management System (MMS). If you know the components of the Exchange that you want to use, and their IP addresses and ports, you can bundle those edge node files now. However, if you are uncertain of those details, you might want to bundle those files after you install {{site.data.keyword.edge_notm}}. For more information, see [Gather edge node files](gather_files.md).


## What's Next

Continue setting up your new management hub by performing the steps in [Install {{site.data.keyword.ieam}}](online_installation.md).
