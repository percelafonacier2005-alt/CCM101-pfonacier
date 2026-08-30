
# Cloud Infrastructure Components

## Compute Resources

### Purpose

Compute resources refer to the processing capacity available in a server. They include the processor and memory used when the system performs operations.

### Why It Is Important

These resources are needed to execute programs, process commands, and support workloads running on the server.

### Relation to the Linux Environment Provided by KillerCoda

The KillerCoda environment allowed me to check the processor, number of CPU cores, and available RAM. The information showed the computing capacity assigned to the Linux server.

## Storage Resources

### Purpose

Storage resources provide space where the operating system, applications, files, and other information can be kept.

### Why It Is Important

A server needs storage to save data and system files so that they can be accessed when needed.

### Relation to the Linux Environment Provided by KillerCoda

I checked the storage using `df -h` and examined the mounted file systems with `findmnt`. From these commands, I was able to see the available disk space and how different file systems were mounted.

## Networking Resources

### Purpose

Networking resources make it possible for computers and cloud services to exchange data and communicate with one another.

### Why It Is Important

A functioning network is needed for servers to communicate with other systems and provide services to users or applications.

### Relation to the Linux Environment Provided by KillerCoda

I used `hostname -I` in the KillerCoda terminal to check the IP addresses assigned to the Linux environment. This gave me a better idea of how the server is identified on the network.

## Operating System

### Purpose

The operating system provides the main environment where system processes, commands, and applications operate.

### Why It Is Important

It manages the server's resources and provides the tools needed to interact with the hardware and software.

### Relation to the Linux Environment Provided by KillerCoda

The Linux environment supplied by KillerCoda uses Ubuntu 24.04.4 LTS. I was able to use the terminal to examine different parts of the system and perform the required investigation.
