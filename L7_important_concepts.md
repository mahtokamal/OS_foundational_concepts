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

# Containerization
Virtualization enables you to run multiple operating systems on the hardware of a single physical server, while containerization enables you to deploy multiple applications using the same operating system on a single virtual machine or server. <br>

Containerization also allows users to run many instances on a single physical host, but it does so without needing the hypervisor to act as an intermediary. Instead, the functionality of the host system kernel is used to isolate multiple independent instances (containers). By sharing the host kernel and operating system, containers avoid the overhead of virtualization, as there’s no need to provide a separate virtual kernel and OS for each instance. This is why containers are considered a more lightweight solution – they require fewer resources without compromising on performance. <br>

# Docker
Docker is an open-source platform for developers to build, deploy, and manage containers. Containers are executable units of software which package and manage the software and components to run a service. They are pretty lightweight because they isolate the application and use the host OS kernel.

# Kubernetes

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

**NoTE:** A virtual machine runs on a hypervisor (software that emulates and manages multiple operating systems on one physical host). It includes a full guest OS, making it heavier but fully isolated. Containers share the host OS kernel, isolating only applications and their dependencies, which makes them lightweight and fast to start. Virtual machines are ideal for running multiple different operating systems or legacy applications, while containers excel at deploying scalable, portable micro-services.

![1715412904464](https://github.com/user-attachments/assets/4e5038ed-ea5d-4a17-9258-c9caffb911a7)
![1669534020612](https://github.com/user-attachments/assets/971929bf-bae0-45dc-b576-708feaf1c96d)
![Container-based-Virtualization-vs-Traditional-Virtualization](https://github.com/user-attachments/assets/abe95e77-808c-45e9-a224-36cc69e99be8)

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# How is virtualization different from cloud computing?
# 1. CPU
## Process, Threads, Handles, Uptime
## Base Speed, Sockets
## Cores, Logical Processors
## Cache L1, L2, L3
## Registers

# 2. Hyperthreading
# 3. Virtual Memory Management
# 4. Buffer Overflow
# 5. Swapping (Swap file)
# 6. Paging (Page file)
# 7. Disk Fragmentation and Defragmentation
# 8. Program
# 9. Process
# 10. Thread vs Multi-threading
# 11. Task
# 12. File Management
# 13. Disk Management
# 14. Process Management
# 15. Memory Management
# 16. User Management
# 17. Resource Management
# 18. Multiprocessing
# 19. Multithreading
# 20. Device Managemnt
# 21. Inter-Process Communication
# 22. Cloud Computing
# 23. Stratup-apps
# 24. Services.msc

# Concepts 1

🏦 Scenario: Online payment in a banking system

A customer clicks “Transfer Money” on a banking app.
Backend runs on servers (e.g., VMs on VMware ESXi, app tier, DB tier like Oracle Database).

We’ll follow that one request through the system.

🧠 1. CPU (Central Processing Unit)

👉 Role: Executes instructions

Inside the system:
CPU fetches instructions → decodes → executes
Handles calculations, logic, data movement
Analogy:

Executive decision-maker

Example:

When calculating new balance after transfer:

new_balance = old_balance - amount

CPU performs this computation.

⚙️ 2. Process

👉 Role: A running program with its own memory space

Inside the system:
Banking backend (Java/.NET service) runs as a process
Database runs as a separate process
Analogy:

A department in a company

Example:
“Payment Service” process
Database process (Oracle Database)
🧵 3. Thread

👉 Role: Unit of execution inside a process

Inside the system:
One process → many threads handling multiple users
Analogy:

Employees inside a department

Example:
Thread 1 → handles User A transfer
Thread 2 → handles User B login

👉 Threads share memory (faster communication)

🔗 4. Handles

👉 Role: References to system resources

Inside the system:
OS assigns handles to access:
Files
Network sockets
Database connections
Analogy:

Access cards / keys

Example:
Handle to:
Transaction log file
TCP connection to user
⏱️ 5. Uptime

👉 Role: Duration system has been running

Inside the system:
Critical for reliability monitoring
Analogy:

How long the bank has stayed open without closing

Example:
Banking server uptime: 180 days
High uptime = stable infrastructure
⚡ 6. Base Speed

👉 Role: Default CPU frequency

Inside the system:
Determines baseline instruction processing rate
Analogy:

Normal working pace of an employee

Example:
CPU base speed: 2.4 GHz
Can boost to 3.5 GHz under load
🔌 7. Sockets

👉 Role: Physical CPU slots on motherboard

Inside the system:
Each socket holds one CPU
Analogy:

Workstations for managers

Example:
2-socket server:
2 CPUs installed (common in enterprise servers from Hewlett Packard Enterprise)
🧩 8. Cores

👉 Role: Independent processing units inside CPU

Inside the system:
Each core executes tasks independently
Analogy:

Multiple managers working simultaneously

Example:
1 CPU with 8 cores → 8 parallel tasks
🔀 9. Logical Processors

👉 Role: Virtual cores (via hyper-threading)

Inside the system:
Each core can handle multiple threads
Analogy:

One manager multitasking between two tasks

Example:
8 cores → 16 logical processors (common in Intel CPUs)
🧠 10. Cache (L1, L2, L3)

👉 Role: Fast memory close to CPU

Inside the system:

When processing a transaction:

CPU checks L1 cache (fastest)
If not found → L2
Then → L3
Then → RAM
Analogy:
L1 → sticky notes on desk
L2 → drawer
L3 → shared cabinet
Example:
Frequently accessed account data stays in cache for quick reuse
📦 11. Registers

👉 Role: Smallest, fastest storage inside CPU

Inside the system:
Holds immediate values during execution
Analogy:

Numbers in your head during calculation

Example:
While subtracting balance:
Amount stored in register
Intermediate result stored in another register
🔄 How everything works together (step-by-step)
💳 User initiates transfer:
1. Request enters system
Network connection created → handle assigned
2. Process handles request
Banking app process receives it
3. Thread executes task
A thread is assigned to this request
4. CPU scheduling
OS assigns thread to:
Core
Possibly a logical processor
5. Execution inside CPU
Instructions processed using:
Registers (immediate values)
Cache (L1/L2/L3) for quick data access
6. Data access
Thread uses handles to:
Read/write database
Log transaction
7. Output generated
Response sent back to user
8. System continues running
Uptime increases

# concepts 2
🧠 1. Hyperthreading

👉 A single CPU core runs multiple threads (logical processors)

Example:
An Intel CPU with 8 cores appears as 16 logical processors.
👉 A web server handles more user requests simultaneously.

💾 3. Virtual Memory Management

👉 Uses disk space as extra RAM

Example:
A banking app exceeds RAM → OS moves inactive data to disk so system doesn’t crash.

⚠️ 4. Buffer Overflow

👉 When a program writes more data than allocated memory

Example:
A login form without limits → attacker sends huge input → overwrites memory → potential security breach.

🔄 5. Swapping (Swap file)

👉 Moves entire processes between RAM and disk

Example:
Low-memory server swaps out an idle reporting process to free RAM for active users.

📄 6. Paging (Page file)

👉 Moves memory in fixed-size chunks (pages)

Example:
Instead of moving full app, OS swaps only required pages → more efficient than swapping.

💽 7. Disk Fragmentation & Defragmentation

👉 Files split across disk → slower access

Example:

Fragmented: file stored in pieces → slow read
Defragmented: stored contiguously → faster

👉 Common in older HDD systems

📦 8. Program

👉 A static file (not running)

Example:
Installer for Microsoft Word sitting on disk

⚙️ 9. Process

👉 A running program

Example:
Opening Word → creates a process in memory

🧵 10. Thread vs Multithreading

👉 Thread = execution unit
👉 Multithreading = multiple threads in one process

Example:
Browser:

One thread loads page
Another loads images
Another handles user input
🧾 11. Task

👉 General term for work being executed

Example:
In Windows Task Manager → each running app is a task

📁 12. File Management

👉 OS organizes and controls files

Example:
Saving reports in folders with permissions (read/write)

💿 13. Disk Management

👉 Managing storage devices

Example:
Creating partitions, formatting drives, assigning letters

⚙️ 14. Process Management

👉 OS controls process lifecycle

Example:

Start app
Allocate CPU
Terminate if needed
🧠 15. Memory Management

👉 Allocates and frees RAM

Example:
Multiple apps running → OS ensures each gets required memory without conflict

👤 16. User Management

👉 Controls users and permissions

Example:

Admin vs normal user
Login authentication in enterprise systems
🔧 17. Resource Management

👉 OS distributes CPU, memory, disk, network

Example:
Database gets more CPU than background apps

⚡ 18. Multiprocessing

👉 Multiple CPUs working together

Example:
Server with 2 CPUs handles thousands of transactions in parallel

🧵 19. Multithreading

👉 Same as above concept (inside process)

Example:
E-commerce app processes multiple orders simultaneously

🔌 20. Device Management

👉 OS controls hardware devices

Example:
Printer drivers, disk drivers, network adapters

🔗 21. Inter-Process Communication (IPC)

👉 Processes communicate with each other

Example:

App server talks to database
Uses sockets, pipes, shared memory
☁️ 22. Cloud Computing

👉 Running apps on remote servers via internet

Example:
Apps hosted on Amazon Web Services or Microsoft Azure

🚀 23. Startup Apps

👉 Programs that start automatically with OS

Example:

Antivirus
Cloud sync tools
⚙️ 24. Services.msc

👉 Windows tool to manage background services

Example:

Start/stop database service
Control system services like Windows Update
🧠 Final mental model

All of these are handled by the Operating System, which acts like a central manager:

Runs programs → processes → threads
Allocates memory & CPU
Manages files, disks, users, and devices
Ensures everything runs efficiently and securely
