# SPS Sandbox
Purpose: 
To quickly demonstrate use case which are not available in democenter and been timeconsuming for custom setup (with CSC)


Out of Scope: 
Any performance test  on Storage array 


	
![image](https://github.com/user-attachments/assets/afcd9d8d-8538-4273-bff9-ca5afdd2e972)

In the initial phase, use case related to Phase I infrastructure are delivered. Use case related to Phase II infra will be delivered by March'25



Usecases: 

Phase I
![image](https://github.com/user-attachments/assets/536db3bd-ae7d-4cdf-912a-cfea3132b48c)

Phase II
		
![image](https://github.com/user-attachments/assets/e413d0ef-bfda-4af9-ae4e-e123fef37233)



# SPS Sandbox

## Purpose:
To quickly demonstrate use cases that are not available in Democenter and have been time-consuming for custom setups (with CSC).

## Out of Scope:
Any performance tests on storage arrays.

In the initial phase, use cases related to Phase I infrastructure are delivered. Use cases related to Phase II infrastructure will be delivered by March 2025.

## Setup

| Phase I                                   | Phase II                                         |
|-------------------------------------------|--------------------------------------------------|
| PowerFlex 4.6 x 2 (PF01 & PF02)           | SUSE Rancher                                     |
| PowerStore 4 x 2 (PowerStore-1 & PowerStore-2) | Ansible / Ansible Modules (Dell Storage)        |
| PowerScale                                | Terraform / Terraform Providers (Dell Storage)   |
| Openshift (2 clusters, v4.17)             | Cloud Native / Stateful Applications / Database (MSSQL, MongoDB) |
| Dell CSI drivers for PowerFlex & PowerStore | GitLab / GitHub                                |
| Dell CSM Replication modules for PowerFlex & PowerStore | Ansible Lint / SonarQube                       |
| Dell CSM Auth module for PowerFlex        | ArgoCD / FluxCD                                  |
| Dell CSM Resiliency module for PowerFlex & PowerStore | Jenkins                                      |

## Use Cases:

| Use Case                        | Storage    | Scope                                                                                       |
|----------------------------------|------------|---------------------------------------------------------------------------------------------|
| **Phase I**                      |            |                                                                                             |
| 1. General Management Capability | PowerFlex  | Demonstrate general management capability including replication through PowerFlex Manager 4.6|
| 2. General Management Capability | PowerStore | Demonstrate general management capability including replication through PowerStore Manager 4 (Block only) |
