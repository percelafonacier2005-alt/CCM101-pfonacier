# Laboratory 03 – Multi-Cloud Explorer

This laboratory focuses on exploring and comparing AWS, Microsoft Azure, and Google Cloud Platform (GCP).

## Linux Server Investigation

For this activity, I used the Ubuntu Linux Playground in KillerCoda to examine the server environment. Several Linux commands were executed to collect information about the operating system, processor, memory, and available storage.

## 1. Operating System Information

*Command:*

cat /etc/os-release

*System Details:*

* *Distribution:* Ubuntu
* *Version:* Ubuntu 24.04.4 LTS
* *Release:* 24.04
* *Codename:* Noble Numbat

The investigation confirmed that the server is using Ubuntu 24.04.4 LTS as its operating system.

### Screenshot

<img width="1917" height="385" alt="killercoda-terminal1" src="https://github.com/user-attachments/assets/8c539abd-3a31-40b5-b316-e961789dd64f" />


---

## 2. Processor Information

*Command:*

lscpu

*System Details:*

* *Architecture:* x86_64
* *Processor:* Intel Xeon E312xx (Sandy Bridge)
* *CPU Count:* 1
* *CPU Speed:* 2.0 GHz

The server is configured with a single Intel Xeon E312xx processor and uses the x86_64 architecture.

### Screenshot

<img width="1920" height="1080" alt="killercoda-terminal2" src="https://github.com/user-attachments/assets/62271298-17c7-4600-bd37-aef643499ab2" />



<img width="1920" height="1080" alt="killercoda-terminal2 1" src="https://github.com/user-attachments/assets/74fccac4-a4f1-4461-8257-4c951eb6bd72" />

---

## 3. Memory Information

*Command:*

free -h

*System Details:*

* *Total RAM:* 1.9 GiB
* *Used:* 418 MiB
* *Free:* 862 MiB
* *Available:* 1.5 GiB
* *Swap:* 1.0 GiB

The server has approximately 1.9 GiB of total RAM. At the time of the investigation, approximately 1.5 GiB was available for use.

### Screenshot

<img width="770" height="120" alt="killlercoda-terminal3" src="https://github.com/user-attachments/assets/76b6a4fe-fcd5-415f-9d41-596627a08e15" />


---

## 4. Storage Information

*Command:*

df -h

*System Details:*

* *Root Filesystem:* 19 GiB
* *Used:* 5.4 GiB
* *Available:* 13 GiB
* *Storage Utilization:* 30%

The main filesystem has a total capacity of 19 GiB. Approximately 13 GiB remains available, indicating that the server still has sufficient storage for a basic workload.

### Screenshot

<img width="1431" height="218" alt="killlercoda-terminal4" src="https://github.com/user-attachments/assets/c21452be-442f-4c98-9ad0-fe1b406f1853" />


---

# Cloud Migration Options

The investigated Ubuntu server could be moved to a cloud environment by using a virtual machine service. The three major cloud providers offer virtual machines capable of running Linux operating systems.

| Cloud Provider  | Equivalent Cloud Service | Main Function                               |
| --------------- | ------------------------ | ------------------------------------------- |
| AWS             | Amazon EC2               | Running Linux-based virtual servers         |
| Microsoft Azure | Azure Virtual Machines   | Deploying Linux virtual machines            |
| Google Cloud    | Compute Engine           | Running configurable Linux virtual machines |

## AWS – Amazon EC2

*Amazon EC2* can be used to recreate the Linux server in the AWS cloud. The virtual machine can be assigned appropriate CPU, memory, and storage resources based on the requirements of the original server.

## Microsoft Azure – Azure Virtual Machines

*Azure Virtual Machines* can also support the Ubuntu server because Azure provides virtual machine configurations for Linux operating systems. The organization can select a VM configuration that is close to the original server's hardware requirements.

## Google Cloud – Compute Engine

*Google Compute Engine* provides another option for migrating the Linux environment. It allows users to create configurable virtual machines with selected processing, memory, and storage resources.

# Migration Assessment

Based on the investigation, the existing server has relatively modest requirements:

* *CPU:* 1 CPU at approximately 2.0 GHz
* *Memory:* 1.9 GiB RAM
* *Storage:* 19 GiB
* *Operating System:* Ubuntu 24.04.4 LTS

Because the workload has low resource requirements, it could be recreated using a small cloud virtual machine. However, the final cloud configuration should be determined by the actual application workload, expected number of users, storage growth, and performance requirements.
