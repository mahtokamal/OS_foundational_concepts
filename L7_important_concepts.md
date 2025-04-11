# Operating System Foundation Concepts Everyone should knonw
# 1. Virtualization vs Conatinerization

**Virtualization -** Virtualization is a technology, which acts as a virtual representation of an actual physical machines. The main goal behind virtualization is, to share the computing resources such as Hardware, CPU, Memory, Server, Network, Software etc.

**How does Virtualization actually works?**
Virtualization utlizies a special kind of software known as hypervisor that enable to create many virtual machines or computer on a single physical computer. The Virtual machine then mimics like a actual computer that use the same physcial machines.

# Hypervisor
A Hypervisor is a software that really assists the virtualization to work. Hypervisor also known as virtual machine monitor (VMM). It acts as an intermediary between the physical computer and virtual computer(machine).
The work of hypervisor is to ensure, control and manage the virtual machines' usage of the physical resources (Memory and CPU) of the host computer.

**Categories of Hypervisor**:
There are 2 categories of Hypervisor available:

**Type-1**
A Type-1, native or bare-metal hypervisors, which are directly installed on computer's hardware without any OS is sitting between them, which means it has a direct access on computer's resources. Thus, it is considered as highly efficient and for this reason, large enterprise applications preferred Type 1 hypervisors. KVM( Kernel-based Virtual Machine ) uses the type 1 hypervisor to host multiple virtual machines on the Linux operating system. Examples of Type-1 hypervisor: VMware ESXi, Microsoft Hyper-V, KVM,Citrix Hypervisor (XenServer).

**Type-2**
A Type-2, embedded or hosted hypervisors, which runs on installed Operating System such as (Windows, MacOS).It is required, when you need to run more than one OS on one machine.
Examples of Type-2 hypervisor: Oracle VirtualBox, VMware Workstation, Microsoft Virtual PC.

# Virtual Machine
After Installation of Hypervisor software (virtualization software, just like another software), we can create multiple virtual machine or computer as per our requirements and each virtual machine has its own configuration and resource to operate like a physical(actual) computer does. The Actual computer is **Host** and the Virtual Computers are **Guests**.

# Conatinerization

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

