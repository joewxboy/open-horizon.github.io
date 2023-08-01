---

copyright:
years: 2020 - 2023
lastupdated: "2023-08-01"
title: Security 

parent: Administering
nav_order: 2
has_children: true
has_toc: false
---

{:new_window: target="blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}
{:child: .link .ulchildlink}
{:childlinks: .ullinks}

# Security 
{: #security}

{{site.data.keyword.edge_notm}} ({{site.data.keyword.ieam}}), based on [Open Horizon ](https://github.com/open-horizon){:target="_blank"}{: .externalLink}, uses several security technologies to ensure that it is secure against attacks and safeguards privacy. For more information about {{site.data.keyword.ieam}} security and roles, see:

* [Security and privacy](./security_privacy.md)
* [Role-based access control](/docs/user_management/rbac.md)
* [{{site.data.keyword.edge_notm}} considerations for GDPR readiness](./gdpr.md)
* [Certificates](../user_management/certificates.md)
* [Disaster recovery](../user_management/disaster_recovery.md)
* [Monitoring management hub components](../user_management/monitoring_infrastructure.md)
{: childlinks}

For more information about creating workload signing keys if you do not already have your own RSA keys, see [Preparing to create an edge service](../developing/service_containers.md). Use these keys to sign services when you publish them to the exchange and enable the {{site.data.keyword.ieam}} agent to verify that it started a valid workload.
