# SPS Sandbox
Purpose: 
To quickly demonstrate use case which are not available in democenter and been timeconsuming for custom setup (with CSC)


Out of Scope: 
Any performance test  on Storage array 


Setup 	
Phase I 	Phase II 
PowerFlex 4.6 x 2 (PF01 & PF02) 	SUSE Rancher 
PowerStore 4 x 2 (PowerStore-1 & PowerStore-2)	Ansible /Ansible Modules (Dell Storage)
PowerScale	Terraform /Terraform Providers (Dell storage)
Openshift (2 clusters, v4.17)	Cloud Native/Stateful Applications /Database (MSSQL, MongoDB ??) 
Dell CSI drivers for PowerFlex & PowerStore	Gitlab/Github
Dell CSM Replication modules for PowerFlex & PowerStore	Ansible lint/Sonarqube
Dell CSM Auth module for PowerFlex	ArgoCD/FluxCD
Dell CSM Resliency module for PowerFlex & PowerStore	Jenkins
	
	
![image](https://github.com/user-attachments/assets/d175bc56-a743-4dee-8a12-c4bf9e681260)
