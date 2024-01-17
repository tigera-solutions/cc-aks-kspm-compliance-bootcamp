# Microsoft AKS Security Bootcamp: <br> Kubernetes Security Posture Management (KSPM) and Compliance

## Welcome

During this workshop, you will learn how to use Azure AKS and Calico Cloud to design and implement best practices for achieving compliance with regulatory frameworks such as PCI, SOC2, and HIPAA. The workshop will cover topics such as Kubernetes Security Posture Management (KSPM), implementing security policies for compliance, and generating evidence and audit reports.

Organizations creating cloud-native applications that meet regulations have two main requirements. The first is to secure and manage access to containerized workloads and the Kubernetes environment. The second is to streamline audit logging and compliance reporting. Kubernetes is a distributed and dynamic environment where workloads are ephemeral. It is challenging to enforce compliance controls and provide consistent reporting.

This repository guides you in creating an Azure AKS cluster, registering it with Calico Cloud, and securing your cloud-native applications to meet compliance standards. While Calico Cloud offers many features, this workshop will focus on only a few key ones due to time limitations. If you would like to learn more about this topic, please feel free to contact us.

## Time Requeriments

The estimated time to complete this workshop is 60-90 minutes.

## Target Audience

- Cloud Professionals
- DevSecOps Professional
- Site Reliability Engineers (SRE)
- Solutions Architects
- Anyone interested in Calico Cloud :)

## Learning Objectives

Learn how to:

- Design and deploy **best practices** to secure your Kubernetes environment in AKS.
- Implement **Kubernetes Security Posture Management** (KSPM) to ensure the overall security of your AKS cluster.
- Create and enforce **security policies** to achieve **compliance** with **regulatory frameworks** such as HIPAA, PCI, SOC 2, and GDPR.
- Generate **evidence** and **audit reports** to demonstrate adherence to compliance requirements.
- Implement **network policies** to control traffic flow and **secure communication** between pods in your AKS cluster.

## Workshop Environment Preparation

> :warning: **For this workshop, you are expected to have access to a previously created AKS cluster.**

- Please, follow the instructions on the repository below if you don't have it ready:

  [Calico Cloud on AKS - Workshop Environment Preparation](https://github.com/tigera-solutions/aks-workshop-prep)

- We will run this workshop from the Azure Cloud Shell, as described in that repository.

- To start your cluster, reload the environment variables create in your Azure Cloud Shell first and then start the cluster. Use the following command:

  ```bash
  source ~/workshopvars.env
  az aks start --resource-group $RESOURCE_GROUP --name $CLUSTERNAME
  ```

## Modules

This workshop is organized in sequencial modules. One module will build up on top of the previous module, so please, follow the order as proposed below.

Module 1 - [Connect the AKS cluster to Calico Cloud](/mod/module-1-connect-calicocloud.md)  
Module 2 - [Security Guardrails for Network-based Threats](/mod/module-2-security-guardrails.md)  
Module 3 - [Configuring IDS protection and Workload-Centric WAF](/mod/module-3-ids-waf.md)  
Module 4 - [Quarantine Infected Workloads and KSPM](/mod/module-4-quarantine-kspm.md)  
Module 5 - [Clean up](/mod/module-5-clean-up.md)  

---

### Useful links

- [Project Calico](https://www.tigera.io/project-calico/)
- [Calico Academy - Get Calico Certified!](https://academy.tigera.io/)
- [O’REILLY EBOOK: Kubernetes security and observability](https://www.tigera.io/lp/kubernetes-security-and-observability-ebook)
- [Calico Users - Slack](https://slack.projectcalico.org/)

### **Follow us on social media**

- [LinkedIn](https://www.linkedin.com/company/tigera/)
- [Twitter](https://twitter.com/tigeraio)
- [YouTube](https://www.youtube.com/channel/UC8uN3yhpeBeerGNwDiQbcgw/)
- [Slack](https://calicousers.slack.com/)
- [Github](https://github.com/tigera-solutions/)
- [Discuss](https://discuss.projectcalico.tigera.io/)

> **Note**: The examples and sample code provided in this workshop are intended to be consumed as instructional content. These will help you understand how Calico Cloud can be configured to build a functional solution. These examples are not intended for use in production environments.
