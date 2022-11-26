# Q.  Define Hypervisior in cloud computing and their types. Describe Hypervisior baseline function. (MAKAUT 2019)

### *What is a Cloud Hypervisor?*
A Cloud Hypervisor is software that enables the sharing of cloud provider’s physical compute and memory resources across multiple virtual machines (VMs). Originally created for mainframe computers in the 1960s, hypervisors gained wide popularity with the introduction of VMware for industry standard servers in the 1990s, enabling a single physical server to independently run multiple guest VMs each with their own operating systems (OSs) that are logically separate from each other. In this manner, problems or crashes in one guest VM have no effect on the other guest VMs, OSs, or the applications running on them.

- Although there are multiple types of VMs, they all perform the same task, enabling a single set of physical server hardware (including CPU, memory, storage, and peripherals) and enabling the simultaneous use by multiple instances of OSs, whether Windows, Linux, or both.

### *What are Types of Hypervisors in Cloud Computing?*
There are two main hypervisor types, referred to as “Type 1”  “bare metal”) and “Type 2” (or “hosted”). A type 1 hypervisor acts like a lightweight operating system and runs directly on the host’s hardware, while a type 2 hypervisor runs as a software layer on an operating system, like other computer programs.

- Cloud providers most commonly deploy a Type 1 or bare-metal hypervisor, where virtualization software is installed directly on the hardware where the operating system is normally installed. Because bare-metal hypervisors are isolated from the attack-prone operating system, they are extremely secure. In addition, they generally perform better and more efficiently than hosted hypervisors. For these reasons, most enterprise companies choose bare-metal hypervisors for data center computing needs.

- While bare-metal hypervisors run directly on the computing hardware, hosted or Type 2 hypervisors run on top of the operating system (OS) of the host machine. Although hosted hypervisors run within the OS, additional (and different) operating systems can be installed on top of the hypervisor. The downside of hosted hypervisors is that latency is higher than bare-metal hypervisors. This is because communication between the hardware and the hypervisor must pass through the extra layer of the OS. Hosted hypervisors are sometimes known as client hypervisors because they are most often used with end users and software testing, where higher latency is less of a concern.

- Both types of hypervisors can run multiple virtual servers for multiple tenants on one physical machine. Public cloud service providers lease server space on the different virtual servers to different companies. One server might host several virtual servers that are all running workloads for different companies. This type of resource sharing can result in a “noisy neighbor” effect, when one of the tenants runs a large workload that interferes with the server performance for other tenants. It also poses more of a security risk than using a dedicated bare-metal server.

### *Hypervisor Baseline Functions*

While the basic function of a hypervisor is to virtualize hardware (a physical host) to enable the operation
of multiple virtual hosts (popularly known as VMs), commercial hypervisor offerings come with differing
feature sets. The modules that provide the same set of features are given different names in different product
offerings. Hence, for accomplishing the goals of this document, it is necessary to identify a set of baseline
features of a hypervisor that covers all functions for supporting hardware virtualization. In some instances,
the module that just presents a set of virtualized resources to the VMs is called the Virtual Machine Manager
(VMM). When VMMs are combined with the modules that provide OS-level services, such as the scheduling
of VMs in the CPU, they are called the hypervisor. These hypervisor baseline features or functions are:

- <b>HY-BF1: VM Process Isolation</b> – Scheduling of VMs for execution, Management of the application
processes running in VMs such as CPU and Memory Management, context switching between various
processor states during the running of applications in VMs, etc.
- <b>HY-BF2: Devices Emulation & Access Control</b> – Emulating all Network and Storage (block) devices
that are expected by different native drivers in VMs, mediating access to physical devices by different
VMs
- <b>HY-BF3: Execution of Privileged Operations for Guest VMs</b> – Execution of certain operations
invoked by Guest OSs by the hypervisor instead of being executed directly by the host hardware because
of their privileged nature; applies to hypervisors that have implemented paravirtualization instead of full
virtualization
- <b>HY-BF4: VM Lifecycle management</b> – All functions including creation and management of VM images,
control of VM states (Start, Pause, Stop, etc.), VM migration, making snapshots, VM monitoring, and
policy enforcement
- <b>HY-BF5: Management of hypervisor</b> – Defining some artifacts and setting values for various
configuration parameters in hypervisor software modules including those for configuration of a Virtual
Network inside the hypervisor and updates and patching to those modules.

### Sources - [Hypervisior Baseline Functions](https://www.govinfo.gov/content/pkg/GOVPUB-C13-03add4670792c21a9d4633fb1b11d3f5/pdf/GOVPUB-C13-03add4670792c21a9d4633fb1b11d3f5.pdf) - [Hypervisior](https://www.vmware.com/topics/glossary/content/cloud-hypervisor.html#:~:text=A%20Cloud%20Hypervisor%20is%20software,multiple%20virtual%20machines%20(VMs).)
