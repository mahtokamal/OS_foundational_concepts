# Operating System Foundation Concepts Everyone should knonw
# 1. Virtualization vs Conatinerization

**Virtualization** <br>
Virtualization is a technology, which acts as a virtual representation of an actual physical machines. The main goal behind virtualization is, to share the computing resources such as Hardware, CPU, Memory, Server, Network, Software etc.

**How does Virtualization actually works?** <br>
Virtualization utlizies a special kind of software known as hypervisor that enable to create many virtual machines or computer on a single physical computer. The Virtual machine then mimics like a actual computer that use the same physcial machines.

# Hypervisor
A Hypervisor is a software that really assists the virtualization to work. Hypervisor also known as virtual machine monitor (VMM). It acts as an intermediary between the physical computer and virtual computer(machine).
The work of hypervisor is to ensure, control and manage the virtual machines' usage of the physical resources (Memory and CPU) of the host computer.

**Categories of Hypervisor**<br>
There are 2 categories of Hypervisor available:

![0_r7b1FbiZM3bdTZDf](https://github.com/user-attachments/assets/62a93392-d9db-458b-bccc-202ed89eaa69)


**Type-1** <br>
A Type-1, native or bare-metal hypervisors, which are directly installed on computer's hardware without any OS is sitting between them, which means it has a direct access on computer's resources. Thus, it is considered as highly efficient and for this reason, large enterprise applications preferred Type 1 hypervisors. KVM( Kernel-based Virtual Machine ) uses the type 1 hypervisor to host multiple virtual machines on the Linux operating system. Examples of Type-1 hypervisor: VMware ESXi, Microsoft Hyper-V, KVM,Citrix Hypervisor (XenServer).

**Type-2**<br>
A Type-2, embedded or hosted hypervisors, which runs on installed Operating System such as (Windows, MacOS).It is required, when you need to run more than one OS on one machine.
Examples of Type-2 hypervisor: Oracle VirtualBox, VMware Workstation, Microsoft Virtual PC.

# Virtual Machine
After Installation of Hypervisor software (virtualization software, just like another software), we can create multiple virtual machine or computer as per our requirements and each virtual machine has its own configuration and resource to operate like a physical(actual) computer does. The Actual computer is **Host** and the Virtual Computers are **Guests**.

# Conatinerization
Virtualization enables you to run multiple operating systems on the hardware of a single physical server, while containerization enables you to deploy multiple applications using the same operating system on a single virtual machine or server. <br>

Containerization also allows users to run many instances on a single physical host, but it does so without needing the hypervisor to act as an intermediary. Instead, the functionality of the host system kernel is used to isolate multiple independent instances (containers). By sharing the host kernel and operating system, containers avoid the overhead of virtualization, as there’s no need to provide a separate virtual kernel and OS for each instance. This is why containers are considered a more lightweight solution – they require fewer resources without compromising on performance. <br>


**Which one to choose?** <br>

Whether you should go for virtualization, containerization or a mix of the two really depends on your use case and needs. Do you need to run multiple applications with different OS requirements? Virtualization is the way to go. Are you building something new from the ground up and want to optimize it for the cloud? Containerization is the choice for you. A lot of the same considerations are needed when choosing your cloud migration strategy.

1. Resource Overhead
   containers share the host system’s operating system, and do not need to run a full operating system, they are significantly more lightweight and consume fewer resources. Virtual machines, on the other hand, each require their own OS, which increases the overhead, especially when many VMs are running on the same host system.
   
2. Startup Time

   In general, containers start up more quickly than VMs, because they don’t have to start up an entire operating system. Virtual machines take much longer to boot up. This means containers are more flexible and can be torn down and restarted whenever needed, supporting immutability, which means that a resource never changes after being deployed.
   
3. Portability

   containers have a slight edge because they package the application and all of its dependencies together into a single unit, which can be run on any system that supports the container platform. Virtual machines, while also portable, are more dependent on the underlying hardware.
   
4. Security Isolation

   In terms of security isolation, virtual machines have the advantage. Because each VM is completely isolated from the host system and other VMs, a security breach in one VM typically does not affect the others (although it is possible to compromise the hypervisor and take control of all VMs on the device). Containers, while isolated from each other, still share the host system’s OS, so a breach in one container could possibly leak to other containers.

5. Scalability and Management
The lightweight nature and rapid startup time offered by containers make them ideal for scaling applications quickly and efficiently. They also lend themselves well to the microservices architecture, which can simplify the management of complex applications. Virtual machines, while also scalable, are more resource-intensive and take longer to start, making them less suitable for microservices and distributed applications.



|Virtualization|Containerization|
|-----|--|
|Legacy Applications|Microservices Architectures|
|Environments Needing Strong Isolation|CI/CD|
|IaaS Scenarios|PaaS Scenarios|

![1715412904464](https://github.com/user-attachments/assets/4e5038ed-ea5d-4a17-9258-c9caffb911a7)
![1669534020612](https://github.com/user-attachments/assets/971929bf-bae0-45dc-b576-708feaf1c96d)
![Container-based-Virtualization-vs-Traditional-Virtualization](https://github.com/user-attachments/assets/abe95e77-808c-45e9-a224-36cc69e99be8)




# How is virtualization different from cloud computing?
# 2. Hyperthreading
# 3. Virtual Memory Management
# 4. Buffer Overflow
# 5. Swapping (Seap file)
# 6. Paging (Page file)
# 7. Disk Fragmentation and Defragmentation
# 8. Program
# 9. Process
# 10. Thread
# 11. Task
# 12. File Management
# 13. Disk Management
# 14. Process Management
# 15. Memory Management
# 16. User Management
# 17. Resource Management
# 18. Multikprocessing
# 19. Multithreading
# 20. Device Managemnt
# 21. Inter-Process Communication
# 22. Cloud Computing

