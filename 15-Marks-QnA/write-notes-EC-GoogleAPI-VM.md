# Q. Write short notes on any three of the following (MAKAUT 2019)
- Amazon EC2
- Google API
- SQL Azure
- Virtual Machine

## 1. *Amazon EC2*
- What is EC2 (AMAZON ELASTIC COMPUTE CLOUD)
- Amazon Elastic Compute Cloud (Amazon EC2) provides scalable computing capacity in the Amazon Web Services (AWS) Cloud. Using Amazon EC2 eliminates your need to invest in hardware up front, so you can develop and deploy applications faster. You can use Amazon EC2 to launch as many or as few virtual servers as you need, configure security and networking, and manage storage. Amazon EC2 enables you to scale up or down to handle changes in requirements or spikes in popularity, reducing your need to forecast traffic.

### *Features of Amazon EC2*
Amazon EC2 provides the following features:

- Virtual computing environments, known as instances

- Preconfigured templates for your instances, known as Amazon Machine Images (AMIs), that package the bits you need for your server (including the operating system and additional software)

- Various configurations of CPU, memory, storage, and networking capacity for your instances, known as instance types

- Secure login information for your instances using key pairs (AWS stores the public key, and you store the private key in a secure place)

- Storage volumes for temporary data that's deleted when you stop, hibernate, or terminate your instance, known as instance store volumes

- Persistent storage volumes for your data using Amazon Elastic Block Store (Amazon EBS), known as Amazon EBS volumes

- Multiple physical locations for your resources, such as instances and Amazon EBS volumes, known as Regions and Availability Zones

- A firewall that enables you to specify the protocols, ports, and source IP ranges that can reach your instances using security groups

- Static IPv4 addresses for dynamic cloud computing, known as Elastic IP addresses

- Metadata, known as tags, that you can create and assign to your Amazon EC2 resources

- Virtual networks you can create that are logically isolated from the rest of the AWS Cloud, and that you can optionally connect to your own network, known as virtual private clouds (VPCs)

## 2. *Google Cloud APIs*
Google Cloud APIs are programmatic interfaces to Google Cloud Platform services. They are a key part of Google Cloud Platform, allowing you to easily add the power of everything from computing to networking to storage to machine-learning-based data analysis to your applications.

### *About Cloud APIs*
Cloud APIs are exposed as network API services to customers, such as Cloud Pub/Sub API. Each Cloud API typically runs on one or more subdomains of googleapis.com, such as pubsub.googleapis.com, and provides both JSON HTTP and gRPC interfaces to clients over public internet and Virtual Private Cloud (VPC) networks. Clients can send HTTP and gRPC requests to Cloud API endpoints directly or by using client libraries.

### *Accessing Cloud APIs*
You can access Cloud APIs from server applications with our client libraries in many popular programming languages, from mobile apps via the Firebase SDKs, or by using third-party clients. You can also access Cloud APIs with the Google Cloud CLI tools or Google Cloud console.

### *TLS encryption*
All Cloud APIs accept only secure requests using TLS encryption.

- If you are using one of our client libraries, in-transit encryption is handled for you by the library.
- If you are using your own gRPC client, you need to authenticate with Google (which requires TLS) following the instructions in the gRPC authentication guide.
- If you are creating your own HTTP client, see our HTTP guidelines.

## 3. *Virtual Machine*

### *What is a virtual machine?*
- A Virtual Machine (VM) is a compute resource that uses software instead of a physical computer to run programs and deploy apps. One or more virtual “guest” machines run on a physical “host” machine.  Each virtual machine runs its own operating system and functions separately from the other VMs, even when they are all running on the same host. This means that, for example, a virtual MacOS virtual machine can run on a physical PC. 

- Virtual machine technology is used for many use cases across on-premises and cloud environments. More recently, public cloud services are using virtual machines to provide virtual application resources to multiple users at once, for even more cost efficient and flexible compute

### *What are virtual machines used for?*
- Virtual machines (VMs) allow a business to run an operating system that behaves like a completely separate computer in an app window on a desktop. VMs may be deployed to accommodate different levels of processing power needs, to run software that requires a different operating system, or to test applications in a safe, sandboxed environment.

- Virtual machines have historically been used for server virtualization, which enables IT teams to consolidate their computing resources and improve efficiency. Additionally, virtual machines can perform specific tasks considered too risky to carry out in a host environment, such as accessing virus-infected data or testing operating systems. Since the virtual machine is separated from the rest of the system, the software inside the virtual machine cannot tamper with the host computer.  

### *How do virtual machines work?*
- The virtual machine runs as a process in an application window, similar to any other application, on the operating system of the physical machine. Key files that make up a virtual machine include a log file, NVRAM setting file, virtual disk file and configuration file. 

### *Advantages of virtual machines*
Virtual machines are easy to manage and maintain, and they offer several advantages over physical machines:   

- VMs can run multiple operating system environments on a single physical computer, saving physical space, time and management costs. 
- Virtual machines support legacy applications, reducing the cost of migrating to a new operating system. For example, a Linux virtual machine running a distribution of Linux as the guest operating system can exist on a host server that is running a non-Linux operating system, such as Windows. 
- VMs can also provide integrated disaster recovery and application provisioning options. 

### *Disadvantages of virtual machines*
- While virtual machines have several advantages over physical machines, there are also some potential disadvantages: 

- Running multiple virtual machines on one physical machine can result in unstable performance if infrastructure requirements are not met. 
- Virtual machines are less efficient and run slower than a full physical computer. Most enterprises use a combination of physical and virtual infrastructure to balance the corresponding advantages and disadvantages.

### Sources 👉 [Amazon EC2](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html) - [Google API](https://cloud.google.com/apis/docs/overview) - [Virtual Machine](https://www.vmware.com/topics/glossary/content/virtual-machine.html)
