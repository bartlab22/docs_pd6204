---
title: "Tanzu Standard Getting Started Guide"
linkTitle: "Tanzu Standard Getting Started Guide"
weight: 20
menu:
  main:
    weight: 20
---
Scratch pad to gather all Tanzu Standard public docs in a one stop page. Next steps would be then to format it so to create a good UX/UI to navigate through it eg collapsible or dynamic based on few options eg what IaaS/Cloud

- [Choose your destination!](#choose-your-destination)
  - [vSphere 7 - vSphere with Tanzu](#vsphere-7---vsphere-with-tanzu)
  - [vSphere 6.7 (and vSphere 7)](#vsphere-67-and-vsphere-7)
  - [AWS](#aws)
  - [Azure](#azure)
  - [VMware Cloud on AWS (VMC)](#vmware-cloud-on-aws-vmc)
  - [Azure VMware Solution (AVS)](#azure-vmware-solution-avs)
- [General](#general)
  - [vSphere with Tanzu](#vsphere-with-tanzu)
  - [Tanzu Kubernetes Grid](#tanzu-kubernetes-grid)
  - [Tanzu Mission Control](#tanzu-mission-control)

# Choose your destination!


## vSphere 7 - vSphere with Tanzu

  - Pre-install steps
    - [Prepare env](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-EE236215-DA4D-4579-8BEB-A693D1882C77.html)
    - Networking (choose one)
      - Use NSX-T Data Center
        - [Pre-reqs](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-B1388E77-2EEC-41E2-8681-5AE549D50C77.html#GUID-B1388E77-2EEC-41E2-8681-5AE549D50C77)
        - [Install and configure](https://docs-staging.vmware.com/en/draft/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-8D0E905F-9ABB-4CFB-A206-C027F847FAAC.html#GUID-8D0E905F-9ABB-4CFB-A206-C027F847FAAC)
      - Use vSphere vDS networking with NSX Advanced Load Balancer (AVI)
        - [Pre-reqs](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-7FF30A74-DDDD-4231-AAAE-0A92828B93CD.html#GUID-7FF30A74-DDDD-4231-AAAE-0A92828B93CD)
        - [Install and configure](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-CBA041AB-DC1D-4EEC-8047-184F2CF2FE0F.html#GUID-CBA041AB-DC1D-4EEC-8047-184F2CF2FE0F)
      - Use vSphere vDS networking with HAProxy
        - [Pre-reqs](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-C86B9028-2701-40FE-BA05-519486E010F4.html)
        - [Install and configure](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-5673269F-C147-485B-8706-65E4A87EB7F0.html)
  - Enable Workload Management (choose one)
    - [Using vSphere Networking](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-8D7D292B-43E9-4CB8-9E20-E4039B80BF9B.html)
    - [Using NSX-T Data Center Networking](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-287138F0-1FFD-4774-BBB9-A1FAB932D1C4.html)
  - Post enable steps
    - [Create content library](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-209AAB32-B2ED-4CDF-AE62-B0FAD9D34C2F.html)
    - [Create vSphere Namespace](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-1544C9FE-0B23-434E-B823-C59EFC2F7309.html)
    - [Register with Tanzu Mission Control](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-ED4417DC-592C-454A-8292-97F93BD76957.html)
  - Deploy Tanzu Kubernetes Clusters
    - [Using kubectl](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-2597788E-2FA4-420E-B9BA-9423F8F7FD9F.html)
    - [Using Tanzu CLI](https://docs-staging.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-tanzu-k8s-clusters-connect-vsphere7.html)
    - [Using Tanzu Mission Control](https://docs.vmware.com/en/VMware-Tanzu-Mission-Control/services/tanzumc-using/GUID-0A1AEC6A-3E5C-424F-8EBC-1DDFC14D2688.html)
  - Next steps
    - [Deploy extensions](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-30C87DC5-51B1-4696-A624-CEA9CF54B63A.html) (optional)
    - [Deploy workloads](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-E217C538-2241-4FD9-9D67-6A54E97CA800.html)

## vSphere 6.7 (and vSphere 7)

  - Pre-install steps
    - [Prepare env](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-vsphere.html)
    - [Install VMware Advanced Load Balancer](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-install-nsx-adv-lb.html)
    - [Install Tanzu CLI](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-install-cli.html)
    - [Identity Management](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-enabling-id-mgmt.html) (optional but recommended)
  - Deploy Management Cluster
    - [Using Installer interface](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-deploy-ui.html), or
    - [Using Tanzu CLI and a config file](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-deploy-cli.html)
  - Post-install steps
    - [Configure Identity Management](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-configure-id-mgmt.html)(optional but recommended)
    - [Register management cluster with Tanzu Mission Control](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-register_tmc.html)
  - Deploy Tanzu Kubernetes Clusters
    - [Using Tanzu CLI](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-tanzu-k8s-clusters-deploy.html)
    - Using Tanzu Mission Control
  - Next steps
    - [Deploy extensions and shared services](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-extensions-index.html) (optional)

## AWS

  - Pre-install steps
    - [Prepare env](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-aws.html)
    - [Install Tanzu CLI](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-install-cli.html)
    - [Identity Management](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-enabling-id-mgmt.html) (optional but recommended)
  - Deploy Management Cluster
    - [Using Installer interface](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-deploy-ui.html), or
    - [Using Tanzu CLI and a config file](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-deploy-cli.html)
  - Post-install steps
    - [Configure Identity Management](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-configure-id-mgmt.html)(optional but recommended)
  - Deploy Tanzu Kubernetes Clusters
    - [Using Tanzu CLI](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-tanzu-k8s-clusters-deploy.html)
  - Next steps
    - [Deploy extensions and shared services](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-extensions-index.html) (optional)

## Azure

  - Pre-install steps
    - [Prepare env](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-azure.html)
    - [Install Tanzu CLI](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-install-cli.html)
    - [Identity Management](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-enabling-id-mgmt.html) (optional but recommended)
  - Deploy Management Cluster
    - [Using Installer interface](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-deploy-ui.html), or
    - [Using Tanzu CLI and a config file](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-deploy-cli.html)
  - Post-install steps
    - [Configure Identity Management](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-configure-id-mgmt.html)(optional but recommended)
  - Deploy Tanzu Kubernetes Clusters
    - [Using Tanzu CLI](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-tanzu-k8s-clusters-deploy.html)
  - Next steps
    - [Deploy extensions and shared services](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-extensions-index.html) (optional)

## VMware Cloud on AWS (VMC)

  - Pre-install steps
    - [Prepare env](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-prepare-maas.html#preparing-vmware-cloud-on-aws-0)
    - Install VMware Advanced Load Balancer (Doc not available yet)
    - [Install Tanzu CLI](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-install-cli.html)
    - [Identity Management](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-enabling-id-mgmt.html) (optional but recommended)
  - Deploy Management Cluster
    - [Using Installer interface](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-deploy-ui.html), or
    - [Using Tanzu CLI and a config file](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-deploy-cli.html)
  - Post-install steps
    - [Configure Identity Management](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-configure-id-mgmt.html)(optional but recommended)
  - Deploy Tanzu Kubernetes Clusters
    - [Using Tanzu CLI](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-tanzu-k8s-clusters-deploy.html)
  - Next steps
    - [Deploy extensions and shared services](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-extensions-index.html) (optional)

## Azure VMware Solution (AVS)

  - Pre-install steps
    - [Prepare env](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-prepare-maas.html#preparing-azure-vmware-solution-on-microsoft-azure-2)
    - [Install Tanzu CLI](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-install-cli.html)
    - [Identity Management](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-enabling-id-mgmt.html) (optional but recommended)
  - Deploy Management Cluster
    - [Using Installer interface](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-deploy-ui.html), or
    - [Using Tanzu CLI and a config file](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-deploy-cli.html)
  - Post-install steps
    - [Configure Identity Management](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-mgmt-clusters-configure-id-mgmt.html)(optional but recommended)
  - Deploy Tanzu Kubernetes Clusters
    - [Using Tanzu CLI](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-tanzu-k8s-clusters-deploy.html)
  - Next steps
    - [Deploy extensions and shared services](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.3/vmware-tanzu-kubernetes-grid-13/GUID-extensions-index.html) (optional)

# General

## vSphere with Tanzu

- [Release Notes](https://docs.vmware.com/en/VMware-vSphere/7.0/rn/vsphere-esxi-vcenter-server-7-vsphere-with-tanzu-release-notes.html)
- [Install Docs](https://docs.vmware.com/en/VMware-vSphere/7.0/vmware-vsphere-with-tanzu/GUID-152BE7D2-E227-4DAA-B527-557B564D9718.html)
- [Download](https://my.vmware.com/web/vmware/downloads/info/slug/datacenter_cloud_infrastructure/vmware_vsphere/7_0)
- [Getting started guide](https://core.vmware.com/resource/vsphere-tanzu-quick-start-guide-v1a)
- [POC guide](https://core.vmware.com/resource/tanzu-proof-concept-guide)

## Tanzu Kubernetes Grid

- [Release Notes](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.2/rn/VMware-Tanzu-Kubernetes-Grid-12-Release-Notes.html)
- [Install Docs](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.2/vmware-tanzu-kubernetes-grid-12/GUID-index.html)
- [Download](https://www.vmware.com/go/get-tkg)

## Tanzu Mission Control

- [Release Notes](https://docs.vmware.com/en/VMware-Tanzu-Mission-Control/services/rn/VMware-Tanzu-Mission-Control-Release-Notes.html)
- [Docs](https://docs.vmware.com/en/VMware-Tanzu-Mission-Control/services/tanzumc-using/GUID-B3349CE8-C98D-4453-9EC8-536A72239F8D.html)