---
layout: col-sidebar
title: OWASP GKE Goat
tags: example-tag
level: 2
type: code
pitch: A very brief, one-line description of your project
---

<p align="center">
  <img src="../www-project-gke-goat/external-images/logo-1.png" alt="Logo" width="500"/>
</p>

OWASP GKE Goat is a hands-on GCP GKE security lab that teaches real-world attack and defense techniques for Google managed Kubernetes clusters.

The lab simulates realistic attack paths and defense mechanisms including misconfigured IAM roles, Workload Identity abuse, GCR/Artifact Registry image backdooring, RBAC privilege escalation, and pod-to-node breakout. Participants walk through both the offensive and defensive scenarios.

**Attack Scenarios (includes CVE-2025-55182):**

**Part 1: Basic GKE Exploitation (Within Cluster)**
* Exploit Next.js Application (CVE-2025-55182 RCE) to gain initial access.
* Post-exploitation from Next.js RCE to establish persistence.
* Privilege escalation via overly permissive RBAC policies.
* Pod-to-node breakout via GCE metadata service.
* Artifact Registry exploitation and Docker layer secrets extraction.
* Data exfiltration from GCS buckets.

**Part 2: GKE to GCP Escalation**
* GCP permission enumeration and exploitation.
* Artifact Registry exploitation by image backdooring.
* Container to host breakout.
* Kubelet exploitation.





## Lab Documentation

> Setup and installation documentation is available. Full walkthrough and detailed attack scenarios are not included in the public release.

* Installation Guide: [https://gkegoat.peachycloudsecurity.com](https://gkegoat.peachycloudsecurity.com)
 

* Alternate Link
  * In case of accessibility issues, use:  
_Coming soon_




#### GCP GKE Exploitation

* Deploying Vulnerable GKE Infrastructure
* Metadata Service Abuse to Steal Credentials
* Web App Exploitation to GCP IAM Compromise
* Container Registry to GKE Cluster Compromise
* Pod-to-Node Breakout in GKE
* Privilege Escalation to Cloud Storage Access and Data Exfiltration
* GCE Instance Cleanup Post Exploit





#### Environment Lifecycle

* Infra Spin-up for Vulnerable GKE Cluster
* Complete Infra Teardown Lab




### RoadMap

* Current State:
    * Created and open-sourced hands-on labs for GCP GKE misconfigurations and vulnerabilities.
    * Developed detailed documentation to accompany lab walkthrough and theoretical concepts.
    * Implementation of initial attack &  defense scenarios with IAM and Kubernetes RBAC.
    * Continue using mdbook for documentation.

* Short-Term Goals:
    * Transition existing infrastructure deployment scripts to Terraform.
    * Update documentation to include images and step-by-step instructions for each lab.
    * Expand the defensive scenarios, adding advance topics such as network policies.
    * Add quizes for interaction.

* Long-Term Objectives:
    * Establish a continuous integration/continuous deployment (CI/CD) pipeline to automate the deployment and teardown of lab environments.
    * Develop a community forum to facilitate participant interaction, knowledge sharing, and collaborative learning.
    * Integrate threat modeling lab for GCP GKE infrastructure using GKE Goat to detect and mitigate proactively.
