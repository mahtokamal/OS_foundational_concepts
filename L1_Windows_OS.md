# 1.0. Windows Background & Versions History
Windows Operating System first launched around 35 years ago in 1985. Since then, many versions and editions are released as per requirements or business need. For example - from Windows 1.0 to today's Windows desktop versions 11 and Windows Server version 2019.
# 1.1. Windows History

# 1.1.1 Disk Operating System
# 1.1.2 Disk Operating System
# 1.1.3 Disk Operating System
# 1.1.4 Operating System Vulnerabilities
Since OS is a System Software that consists of millions line of codes and some code might have vulnerabilities.
Vulnerabilities are design flaw or weakness that an attacker can take adavantage of these flaws using some tools and techniques to exploit the System. The main goal is to gain unauthorized access for malicious or illegal purposes such
as manipulation or stealing of data, changing permission or ownerships.

Following are the some of the common Windows OS security recommendations:-
1. Virus or Malware Protection
   - By default, Windows uses Windows Defender for malware protection.
   - Windows Defender provides a suite of protection tools built into the system.
   - If Windows Defender is turned off, the system becomes more vulnerable to attacks and malware.
2. Unknown or unmanaged services
   - There are many services that run behind the scenes.
   - It is important to make sure that each service is identifiable and safe.
   - With an unknown service running in the background, the computer can be vulnerable to attack.
3. Encryptions
   - When data is not encrypted, it can easily be gathered and exploited.
   - This is not only important for desktop computers, but especially mobile devices.
4. Security Policy
   - A good security policy must be configured and followed.
   - Many settings in the Windows Security Policy control can prevent attacks.
5. Firewall
    - By default, Windows uses Windows Firewall to limit communication with devices on the network.
    - Over time, rules may no longer apply.
    - For example, a port may be left open that should no longer be readily available.
    - It is important to review firewall settings periodically to ensure that the rules are still applicable and remove any 
      that no longer apply
6. File and Share Permission
    - These permissions must be set correctly.
    - It is easy to just give the “Everyone” group Full Control, but this allows all people to do what they want to all 
      files.
    - It is best to provide each user or group with the minimum necessary permissions for all files and folders.
8. Weak or no password
    - Many people choose weak passwords or do not use a password at all.
    - It is especially important to make sure that all accounts, especially the Administrator account, have a very strong 
      password.
13. Login as Administrator
    - When a user logs in as an administrator, any program that they run will have the privileges of that account.
    - It is best to log in as a Standard User and only use the administrator password to accomplish certain tasks.

# 1.2. Windows Architecture and Operations

# 1.2.1 HAL (Hardware Abstraction Layers)
![Screenshot (703)](https://github.com/user-attachments/assets/2d72a147-5eb3-4181-9543-2e267d703600)

# 1.2.2 User Mode and Kernel Mode
![Screenshot (704)](https://github.com/user-attachments/assets/9fb627f4-ab35-4b15-91e6-ce599d08f754)

# 1.2.3 Windows File System
1. eXFAT
- This is a simple file system supported by many different operating systems.
- FAT has limitations to the number of partitions, partition sizes, and file sizes that it can address, so it is not usually used for hard drives (HDs) or solid-state drives (SSDs) anymore.
- Both FAT16 and FAT32 are available to use, with FAT32 being the most common because it has many fewer restrictions than FAT16.

2. Hierarchicsl File System (HFS+)
- This file system is used on MAC OS X computers and allows much longer filenames, file sizes, and partition sizes than previous file systems.
- Although it is not supported by Windows without special software, Windows is able to read data from HFS+ partitions.

3. Extended Files System (EXT)
- This file system is used with Linux-based computers.
- Although it is not supported by Windows, Windows is able to read data from EXT partitions with special software.

4. New Technology File System (NTFS)
This is the most commonly used file system when installing Windo NTFS also tracks many time stamps to track file activity. Sometimes referred to as MACE, the timestamps Modify, Access, Create, and Entry Modified are often used in forensic investigations to determine the history of a file or folder. NTFS also supports file system encryption to secure the entire storage media.ws. All versions of Windows and Linux support NTFS.
Mac-OS X computers can only read an NTFS partition. They are able to write to an NTFS partition after installing special drivers.


**NTFS Features:**
1. NTFS supports very large files and partitions and it is very compatible with other operating systems.
2. NTFS is also very reliable and supports recovery features.
3. it supports many security features. Data access control is achieved through security descriptors. These security descriptors contain file ownership and permissions all the way down to the file level.
4. These security descriptors contain file ownership and permissions all the way down to the file level. NTFS also tracks many time stamps to track file activity. Sometimes referred to as MACE, the timestamps Modify, Access, Create, and Entry Modified are often used in forensic investigations to determine the history of a file or folder.
5. NTFS also supports file system encryption to secure the entire storage media.


NTFS formatting creates important structures on the disk for file storage, and tables for recording the locations of files:

- **Partition Boot Sector** - This is the first 16 sectors of the drive. It contains the location of the Master File Table (MFT). The last 16 sectors contain a copy of the boot sector.
- **Master File Table (MFT)** - This table contains the locations of all the files and directories on the partition, including file attributes such as security information and timestamps.
- **System Files** - These are hidden files that store information about other volumes and file attributes.
- **File Area** - The main area of the partition where files and directories are stored.

**Note:** When formatting a partition, the previous data may still be recoverable because not all the data is completely removed. The free space can be examined, and files can be retrieved which can compromise security. It is recommended to perform a secure wipe on a drive that is being reused. The secure wipe will write data to the entire drive multiple times to ensure there is no remaining data.

# 1.2.4 Aternate Data Streams (ADS)
NTFS stores files as a series of attributes, such as the name of the file, or a timestamp. The data which the file contains is stored in the attribute $DATA, and is known as a data stream. By using NTFS, you can connect Alternate Data Streams (ADSs) to the file. This is sometimes used by applications that are storing additional information about the file. The ADS is an important factor when discussing malware. This is because it is easy to hide data in an ADS. An attacker could store malicious code within an ADS that can then be called from a different file.

In the NTFS file system, a file with an ADS is identified after the filename and a colon, for example, Testfile.txt:ADS. This filename indicates an ADS called ADS is associated with the file called Testfile.txt. An example of ADS is shown in the command output.

![Screenshot (705)](https://github.com/user-attachments/assets/78242cad-4039-49a5-834a-992c19bd6d8f)

In the output:
- The first command places the text “Alternate Data Here” into an ADS of the file Testfile.txt called “ADS”.
- After that, dir, shows that the file was created, but the ADS is not visible.
- The next command shows that there is data in the Testfile.txt:ADS data stream.
- The last command shows the ADS of the Testfile.txt file because the r switch was used with the dir command.

# 1.2.5 Windows Boot Process

# 1.2.6 Windows Startup
There are two important registry items that are used to automatically start applications and services:

- **HKEY_LOCAL_MACHINE** - Several aspects of Windows configuration are stored in this key, including information about services that start with each boot.
- **HKEY_CURRENT_USER** - Several aspects related to the logged in user are stored in this key, including information about services that start only when the user logs on to the computer.

Different entries in these registry locations define which services and applications will start, as indicated by their entry type. These types include Run, RunOnce, RunServices, RunServicesOnce, and Userinit. These entries can be manually entered into the registry, but it is much safer to use the **Msconfig.exe tool**. This tool is used to view and change all of the start-up options for the computer. Use the search box to find and open the Msconfig tool.

The Msconfig tool opens the System Configuration window. There are five tabs which contain the configuration options.

1. General
Three different startup types can be chosen here. Normal loads all drivers and services. Diagnostic loads only basic drivers and services. Selective allows the user to choose what to load on startup.
![Screenshot (706)](https://github.com/user-attachments/assets/1a891afc-b4b9-452c-89fa-a770ea514f18)

2. Boot
Any installed operating system can be chosen here to start. There are also options for Safe boot, which is used to troubleshoot startup.
![Screenshot (707)](https://github.com/user-attachments/assets/223ed78b-1c67-46a3-b371-b36d0c48f7a9)

3. Services
All the installed services are listed here so that they can be chosen to start at startup.
![Screenshot (708)](https://github.com/user-attachments/assets/ea91d991-f604-4252-bf4b-625150a0d1e0)

4. Startup
All the applications and services that are configured to automatically begin at startup can be enabled or disabled by opening the task manager from this tab.
![Screenshot (709)](https://github.com/user-attachments/assets/15f3d2e0-dbe4-4b98-99aa-d4c92b148e47)

5. Tools
   Many common operating system tools can be launched directly from this tab.
![Screenshot (710)](https://github.com/user-attachments/assets/452cb479-e1c1-422b-aadc-fa99e12ca59b)

# 1.2.7 Windows Shutdown
It is always best to perform a proper shutdown to turn off the computer. Files that are left open, services that are closed out of order, and applications that hang can all be damaged if the power is turned off without first informing the operating system. The computer needs time to close each application, shut down each service, and record any configuration changes before power is lost.

During shutdown, the computer will close user mode applications first, followed by kernel mode processes. If a user mode process does not respond within a certain amount of time, the OS will display notification and allow the user to wait for the application to respond, or forcibly end the process. If a kernel mode process does not respond, the shutdown will appear to hang, and it may be necessary to shut down the computer with the power button.

There are several ways to shut down a Windows computer: Start menu power options, the command line command shutdown, and using Ctrl+Alt+Delete and clicking the power icon. There are three different options from which to choose when shutting down the computer:

- **Shutdown** - Turns the computer off (power off).
- **Restart**- Re-boots the computer (power off and power on).
- **Hibernate** - Records the current state of the computer and user environment and stores it in a file. Hibernation allows users to pick up right where they left off very quickly with all their files and programs still open.


# 1.2.8 Processes, Threads, and Services
A Windows application is made up of processes. The application can have one or many processes dedicated to it. A process is any program that is currently executing. Each process that runs is made up of at least one thread. A thread is a part of the process that can be executed. The processor performs calculations on the thread. To configure Windows processes, search for Task Manager. The Processes tab of the Task Manager is shown in the figure.

![Screenshot (712)](https://github.com/user-attachments/assets/9fca9e85-e275-4150-8d72-4a3be79d094f)

All of the threads dedicated to a process are contained within the same address space. This means that these threads may not access the address space of any other process. This prevents corruption of other processes. Because Windows multitasks, multiple threads can be executed at the same time. The amount of threads that can be executed at the same time is dependent on the number of the computer’s processors.

Some of the processes that Windows runs are services. These are programs that run in the background to support the operating system and applications. They can be set to start automatically when Windows boots or they can be started manually. They can also be stopped, restarted, or disabled.

Services provide long-running functionality, such as wireless or access to an FTP server. To configure Windows Services, search for services. The Windows Services control panel applet is shown in the figure.

![Screenshot (713)](https://github.com/user-attachments/assets/125272a4-e918-435f-9dd2-47a3dc58b3d7)

Be very careful when manipulating the settings of these services. Some programs rely on one or more services to operate properly. Shutting down a service may adversely affect applications or other services.

Program -
Process -
Thread -
# 1.2.9 Memory Allocation and Handles
A computer works by storing instructions in RAM until the CPU processes them. The virtual address space for a process is the set of virtual addresses that the process can use. The virtual address is not the actual physical location in memory, but an entry in a page table that is used to translate the virtual address into the physical address.

Each process in a 32-bit Windows computer supports a virtual address space that enables addressing up to 4 gigabytes. Each process in a 64-bit Windows computer supports a virtual address space of 8 terabytes.

Each user space process runs in a private address space, separate from other user space processes. When the user space process needs to access kernel resources, it must use a process handle. This is because the user space process is not allowed to directly access these kernel resources. The process handle provides the access needed by the user space process without a direct connection to it.

A powerful tool for viewing memory allocation is **RAMMap**, which is shown in the figure. RAMMap is part of the Windows Sysinternals Suite of tools. It can be downloaded from Microsoft. RAMMap provides a wealth of information regarding how Windows has allocated system memory to the kernel, processes, drivers, and applications.
![Screenshot (714)](https://github.com/user-attachments/assets/9b14f4e7-0efb-4b37-836c-4d275f7530c2)

# 1.2.10 The Windows Registry
Windows stores all of the information about hardware, applications, users, and system settings in a **large database** known as the **registry**. The ways that these objects interact are also recorded, such as what files an application opens and all of the property details of folders and applications. The registry is a hierarchical database where the highest level is known as a **hive**, below that there are **keys**, followed by **subkeys**. Values store data and are stored in the keys and subkeys. A registry key can be up to 512 levels deep.

- HEKY_CURRENT_USER (HKCU)
  Holds information concerning the currently logged in user.
- HKEY_USERS (HKU)
  Holds information concerning all the user accounts on the host.
- HKEY_CLASSES_ROOT_ (HKCR)
  Holds information about object linking and embedding (OLE) registrations. OLE allows users to embed objects from other applications (like a spreadsheet) into a single document (like a Word document).
- HKEY_LOCAL_MACHINE (HKLM)
  Holds system-related information.
- HKEY_CURRENT_CONFIG (HKCC)
  Holds information about the current hardware profile.

New hives cannot be created. The registry keys and values in the hives can be created, modified, or deleted by an account with administrative privileges. As shown in the figure, the tool **regedit.exe** is used to modify the registry. Be very careful when using this tool. Minor changes to the registry can have massive or even catastrophic effects.
![Screenshot (715)](https://github.com/user-attachments/assets/9091da61-cdf2-4438-96cf-2a80005703f9)
![Screenshot (716)](https://github.com/user-attachments/assets/adaebae6-0177-4ae3-97cb-b6422f56191b)

Navigation in the registry is very similar to Windows file explorer. Use the left panel to navigate the hives and the structure below it and use the right panel to see the contents of the highlighted item in the left panel. With so many keys and subkeys, the key path can become very long. The path is displayed at the bottom of the window for reference. Because each key and subkey is essentially a container, the path is represented much like a folder in a file system. The backslash (∖) is used to differentiate the hierarchy of the database.

Registry keys can contain either a subkey or a value. The different values that keys can contain are as follows:

- REG_BINARY - Numbers or Boolean values
- REG_DWORD - Numbers greater than 32 bits or raw data
- REG_SZ - String values

Because the registry holds almost all the operating system and user information, it is critical to make sure that it does not become compromised. Potentially malicious applications can add registry keys so that they start when the computer is started. During a normal boot, the user will not see the program start because the entry is in the registry and the application displays no windows or indication of starting when the computer boots. A keylogger, for example, would be devastating to the security of a computer if it were to start at boot without the user’s knowledge or consent. When performing normal security audits, or remediating an infected system, review the application startup locations within the registry to ensure that each item is known and safe to run.

The registry also contains the activity that a user performs during normal day-to-day computer use. This includes the history of hardware devices, including all devices that have been connected to the computer including the name, manufacturer and serial number. Other information, such as what documents a user and program have opened, where they are located, and when they were accessed is stored in the registry. This is all very useful information when a forensics investigation needs to be performed.

# 1.3. Windows Configurations and Monitoring
# 1.3.1 Run as Administrsator
As a security best practice, it is not advisable to log on to Windows using the Administrator account or an account with administrative privileges. This is because any program that is executed while logged on with those privileges will inherit administrative privileges. Malware that has administrative privileges has full access to all the files and folders on the computer.

Sometimes, it is necessary to run or install software that requires the privileges of the Administrator. To accomplish this, there are two different ways to install it.

- **Administrator** -
  Right-click the command in the Windows File Explorer and choose Run as Administrator from the Context Menu.

![Screenshot (717)](https://github.com/user-attachments/assets/e552ec0f-64c3-4536-a4fc-76a72bd0cd13)

- **Administrator Command Prompt** -
  Search for command, right-click the executable file, and choose Run as Administrator from the Context Menu. Every command that is executed from this command line will be carried out with the Administrator privileges, including installation of software.
  
![Screenshot (718)](https://github.com/user-attachments/assets/e9a5ea64-e003-4011-b887-72b589454a93)

# 1.3.2 Local Users and Domains
When you start a new computer for the first time, or you install Windows, you will be prompted to create a user account. This is known as a local user. This account will contain all of your customization settings, access permissions, file locations, and many other user-specific data. There are also two other accounts that are present, the guest, and the administrator. Both of these accounts are disabled by default.

As a security best practice, do not enable the Administrator account and do not give standard users administrative privileges. If a user needs to perform any function that requires administrative privileges, the system will ask for the Administrator password and allow only that task to be performed as an administrator. Requiring the administrator password protects the computer by preventing any software that is not authorized from installing, executing, or accessing files.

The Guests account should not be enabled. The guest account does not have a password associated with it because it is created when a computer is going to be used by many different people who do not have accounts on the computer. Each time the guest account logs on, a default environment is provided to them with limited privileges.

To make administration of users easier, Windows uses groups. A group will have a name and a specific set of permissions associated with it. When a user is placed into a group, the permissions of that group are given to that user. A user can be placed into multiple groups to be provided with many different permissions. When the permissions overlap, certain permissions, like “explicitly deny” will override the permission provided by a different group. There are many different user groups built into Windows that are used for specific tasks. For example, the Performance Log Users group allows members to schedule logging of performance counters and collect logs either locally or remotely. Local users and groups are managed with the lusrmgr.msc control panel applet, as shown in the figure.



In addition to groups, Windows can also use domains to set permissions. A domain is a type of network service where all of the users, groups, computers, peripherals, and security settings are stored on and controlled by a database. This database is stored on special computers or groups of computers called domain controllers (DCs). Each user and computer on the domain must authenticate against the DC to logon and access network resources. The security settings for each user and each computer are set by the DC for each session. Any setting supplied by the DC defaults to the local computer or user account setting.
# 1.3.3 CLI and PowerShell

The Windows command line interface (CLI) can be used to run programs, navigate the file system, and manage files and folders. In addition, files called batch files can be created to execute multiple commands in succession, much like a basic script.

To open the Windows CLI, search for cmd.exe and click the program. Remember that right-clicking the program provides the option to Run as administrator, giving much more power to the commands that will be used.

The prompt displays the current location within the file system. These are a few things to remember when using the CLI:

The file names and paths are not case-sensitive, by default.
Storage devices are assigned a letter for reference. The drive letter is followed by a colon and backslash (∖). This indicates the root, or highest level, of the device. Folder and file hierarchy on the device is indicated by separating them with the backslash. For example, the path C:∖Users∖Jim∖Desktop∖file.txt refers to a file called file.txt that is in the Desktop folder within the Jim folder within the Users folder at the root of drive C:.
Commands that have optional switches use the forward slash (/) to delineate between the command and the switch option.
You can use the Tab key to auto-complete commands when directories or files are referenced.
Windows keeps a history of the commands that were entered during a CLI session. Access previously entered commands by using the up and down arrow keys.
To switch between storage devices, type the letter of the device, followed by a colon, and then press Enter.
Even though the CLI has many commands and features, it cannot work together with the core of Windows or the GUI. Another environment, called the Windows PowerShell, can be used to create scripts to automate tasks that the regular CLI is unable to create. PowerShell also provides a CLI for initiating commands. PowerShell is an integrated program within Windows and can be opened by searching for “powershell” and clicking the program. Like the CLI, PowerShell can also be run with administrative privileges.

These are the types of commands that PowerShell can execute:

- cmdlets - These commands perform an action and return an output or object to the next command that will be executed.
- PowerShell scripts - These are files with a .ps1 extension that contain PowerShell commands that are executed.
- PowerShell functions - These are pieces of code that can be referenced in a script.

To see more information about Windows PowerShell and get started using it, type help in PowerShell, as shown in the command output.

![Screenshot (719)](https://github.com/user-attachments/assets/a634939a-a409-4862-9dd8-a6a617e3f517)

There are four levels of help in Windows PowerShell:

get-help PS command - Displays basic help for a command
get-help PS command [-examples] - Displays basic help for a command with examples
get-help PS command [-detailed] - Displays detailed help for a command with examples
get-help PS command [-full] - Displays all help information for a command with examples in greater depth

# 1.3.4 Windows Management Intruementations
Windows Management Instrumentation (WMI) is used to manage remote computers. It can retrieve information about computer components, hardware and software statistics, and monitor the health of remote computers. To open the WMI control from the Control Panel, double-click Administrative Tools > Computer Management to open the Computer Management window, expand the Services and Applications tree and right-click the WMI Control icon > Properties.

The WMI Control Properties window is shown in the figure.

![f08e9200-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/eb930a16-1d5d-440d-ae78-44e3d795ccd3)

These are the four tabs in the WMI Control Properties window:

- **General** - Summary information about the local computer and WMI
- **Backup/Restore** - Allows manual backup of statistics gathered by WMI
- **Security** - Settings to configure who has access to different WMI statistics
- **Advanced** - Settings to configure the default namespace for WMI

Some attacks today use WMI to connect to remote systems, modify the registry, and run commands. WMI helps them to avoid detection because it is common traffic, most often trusted by the network security devices and the remote WMI commands do not usually leave evidence on the remote host. Because of this, WMI access should be strictly limited.

# 1.3.5 The net Command

Windows has many commands that can be entered at the command line. One important command is the net command, which is used in the administration and maintenance of the OS. The net command supports many subcommands that follow the net command and can be combined with switches to focus on specific output.

To see a list of the many net commands, type net help at the command prompt. The command output shows the commands that the net command can use. To see verbose help about any of the net commands, type C:∖> net help ,as shown below.

![Screenshot (721)](https://github.com/user-attachments/assets/4f5e5fd8-013f-4f59-a382-dac143134e60)

- net accounts

  Sets password and logon requirements for users

- net session
  
  Lists or disconnects sessions between a computer and other computers on the network

- net share
  
  Creates, removes, or manages shared resources

- net start
  
  Starts a network service or lists running network services

- net stop

  Stops a network service

- net use

  Connects, disconnects, and displays information about shared network resources

- net view

  Shows a list of computers and network devices on the network

# 1.3.6 Task Manager and Resource Monitor

There are two very important and useful tools to help an administrator to understand the many different applications, services, and processes that are running on a Windows computer. These tools also provide insight into the performance of the computer, such as CPU, memory, and network usage. These tools are especially useful when investigating a problem where malware is suspected. When a component is not performing the way that it should be, these tools can be used to determine what the problem might be.

**Task Manager**

The Task Manager, which is shown in the figure, provides a lot of information about the software that is running and the general performance of the computer.

![f0926290-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/74b2a010-a2e1-41e9-99eb-53e8db977ea9)

Processes

- Lists all of the programs and processes that are currently running.
- Displays the CPU, memory, disk, and network utilization of each process.
- The properties of a process can be examined or ended if it is not behaving properly or has stalled.

Performance

- A view of all the performance statistics provides a useful overview of the CPU, memory, disk, and network performance.
- Clicking each item in the left pane will show detailed statistics of that item in the right pane.

App history

- The use of resources by application over time provides insight into applications that are consuming more resources than they should.
- Click Options and Show history for all processes to see the history of every process that has run since the computer was started.

Startup

- All of the applications and services that start when the computer is booted are shown in this tab.
- To disable a program from starting at startup, right-click the item and choose Disable

Users

- All of the users that are logged on to the computer are shown in this tab.
- Also shown are all the resources that each user’s applications and processes are using.
- From this tab, an administrator can disconnect a user from the computer.

Details

- Similar to the Processes tab, this tab provides additional management options for processes such as setting a priority to make the processor devote more or less time to a process.
- CPU affinity can also be set which determines which core or CPU a program will use.
- Also, a useful feature called Analyze wait chain shows any process for which another process is waiting.
- This feature helps to determine if a process is simply waiting or is stalled.

Services

- All the services that are loaded are shown in this tab.
- The process ID (PID) and a short description are also shown along with the status of either Running or Stopped.
- At the bottom, there is a button to open the Services console which provides additional management of services.

**Resource Monitor**

When more detailed information about resource usage is needed, you can use the Resource Monitor, as shown in the figure.

![f0948570-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/f842e807-9acc-4a7b-8c0c-75012cfef815)

When searching for the reason a computer may be acting erratically, the Resource Monitor can help to find the source of the problem.

**The table describes the five tabs of the Resource Monitor.**

Overview

- The tab displays the general usage for each resource.
- If you select a single process, it will be filtered across all of the tabs to show only that process’s statistics.

CPU

- The PID, number of threads, which CPU the process is using, and the average CPU usage of each process is shown.
- Additional information about any services that the process relies on, and the associated handles and modules can be seen by expanding the lower rows.

Memory

- All of the statistical information about how each process uses memory is shown in this tab.
- Also, an overview of usage of all the RAM is shown below the Processes row.

Disk

- All of the processes that are using a disk are shown in this tab, with read/write statistics and an overview of each storage device.

Network

- All of the processes that are using the network are shown in this tab, with read/write statistics.
- Most importantly, the current TCP connections are shown, along with all of the ports that are listening.
- This tab is very useful when trying to determine which applications and processes are communicating over the network.
- It makes it possible to tell if an unauthorized process is accessing the network, listening for a communication, and the address with which it is communicating.


# 1.3.7 Networking

One of the most important features of any operating system is the ability for the computer to connect to a network. Without this feature, there is no access to network resources or the internet. To configure Windows networking properties and test networking settings, the Network and Sharing Center is used. The easiest way to run this tool is to search for it and click it. Use the Network and Sharing Center to verify or create network connections, configure network sharing, and change network adapter settings.

**Network and Sharing Center**

![f0968140-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/79916749-fbd8-4fc7-a1ab-7a8119a817dc)


**Change Adapter Settings**

To configure a network adapter, choose Change adapter settings in the Networking and Sharing Center to show all of the network connections that are available. Select the adapter that you want to configure. In this case, we change an Ethernet adapter to acquire its IPv4 address automatically from the network.

Access Adapter Properties

Right-click the adapter you wish to configure and choose Properties, as shown in the figure.

![f099dca0-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/9e5c7ccd-3a40-44e6-b8ee-d1a071f26c65)

Access TCP/IPV4 Properties

This connection uses the following items: Internet Protocol Version 4 (TCP/IPv4) or Internet Protocol Version 6 (TCP/IPv6) depending on which version you wish to use. In the figure, IPv4 is being selected.

![f09b8a50-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/81a5313f-9077-4211-80bc-1c35d6769a36)

Change Settings

Click Properties to configure the adapter. In the Properties dialogue box, shown in the figure, you can choose to Obtain an address automatically if there is a DHCP server available on the network. If you wish to configure addressing manually, you can fill in the address, subnet, default gateway, and DNS servers to configure the adapter. Click OK to accept the changes. You can also use the netsh.exe tool to configure networking parameters from a command prompt. This program can display and modify the network configuration. Type netsh /? at the command prompt to see a list of all the switches that can be used with this command.

![f09b8a50-a1fb-11ea-bb42-49e522ad4be8 (1)](https://github.com/user-attachments/assets/22ed856e-3ca8-44b0-8fc2-9a6e9b9a7be6)

**nslookup and netstat**

Domain Name System (DNS) should also be tested because it is essential to finding the address of hosts by translating it from a name, such as a URL. Use the nslookup command to test DNS. Type nslookup cisco.com at the command prompt to find the address of the Cisco webserver. When the address is returned, you know that DNS is functioning correctly. You can also check to see what ports are open, where they are connected, and what their current status is. Type netstat at the command line to see details of active network connections, as shown in the command output. The netstat command will be examined further later in this module

![Screenshot (722)](https://github.com/user-attachments/assets/75fb46b1-6fb4-4826-97c2-8050fd1cda61)

# 1.3.8 Accessing Network Resources

Like other operating systems, Windows uses networking for many different applications such as web, email, and file services. Originally developed by IBM, Microsoft aided in the development of the Server Message Block (SMB) protocol to share network resources. SMB is mostly used for accessing files on remote hosts. The Universal Naming Convention (UNC) format is used to connect to resources, for example:

**∖∖servername∖sharename∖file**

In the UNC, servername is the server that is hosting the resource. This can be a DNS name, a NetBIOS name, or simply an IP address. The sharename is the root of the folder in the file system on the remote host, while the file is the resource that the local host is trying to find. The file may be deeper within the file system and this hierarchy will need to be indicated.

When sharing resources on the network, the area of the file system that will be shared will need to be identified. Access control can be applied to the folders and files to restrict users and groups to specific functions such as read, write, or deny. There are also special shares that are automatically created by Windows. These shares are called administrative shares. An administrative share is identified by the dollar sign ($) that comes after the share name. Each disk volume has an administrative share, represented by the volume letter and the $ such as C$, D$, or E$. The Windows installation folder is shared as admin$, the printers’ folder is shared as print$, and there are other administrative shares that can be connected. Only users with administrative privileges can access these shares.

The easiest way to connect to a share is to type the UNC of the share into the Windows File Explorer, in the box at the top of the screen which shows the breadcrumb listing of the current file system location. When Windows tries to connect to the share, you will be asked to provide credentials for accessing the resource. Remember that because the resource is on a remote computer, the credentials need to be for the remote computer, not the local computer.

Besides accessing shares on remote hosts, you can also log in to a remote host and manipulate that computer, as if it were local, to make configuration changes, install software, or troubleshoot an issue. In Windows, this feature uses the Remote Desktop Protocol (RDP). When investigating security incidents, a security analyst uses RDP often to access remote computers. To start RDP and connect to a remote computer, search for remote desktop and click the application. The Remote Desktop Connection window is shown in the figure.

Because RDP is designed to permit remote users to control individual hosts, it is a natural target for threat actors. Care should be taken when activating RDP, especially on unpatched legacy versions of Windows such as those that are still found in industrial control systems. Care should be taken to limit the exposure of RDP to the internet, and security approaches and access control policies, such as Zero Trust, should be used to limit access to internal hosts.

![f09f33d0-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/7982375a-f053-4e2e-9114-899c9dadc171)

# 1.3.9 Windows Server

Most Windows installations are performed as desktop installations on desktops and laptops. There is another edition of Windows that is mainly used in data centers called Windows Server. This is a family of Microsoft products that began with Windows Server 2003. Windows Server hosts many different services and can fulfill different roles within a company.

**Note:** Although there is a Windows Server 2000, it is considered a client version of Windows NT 5.0. Windows Server 2003 is a server based on NT 5.2 and begins a new family of Windows Server versions.

These are some of the services that Windows Server provides:

- **Network Services** - DNS, DHCP, Terminal services, Network Controller, and Hyper-V Network virtualization

- **File Services** - SMB, NFS, and DFS

- **Web Services** - FTP, HTTP, and HTTPS

- **Management** - Group policy and Active Directory domain services control

# 1.4. Windows Security
# 1.4.1 The netstat Command

When malware is present in a computer, it will often open communication ports on the host to send and receive data. The netstat command can be used to look for inbound or outbound connections that are not authorized. When used on its own, the netstat command will display all of the active TCP connections.

By examining these connections, it is possible to determine which of the programs are listening for connections that are not authorized. When a program is suspected of being malware, a little research can be performed to determine its legitimacy. From there, the process can be shut down with Task Manager, and malware removal software can be used to clean the computer.

To make this process easier, you can link the connections to the running processes that created them in Task Manager. To do this, open a command prompt with administrative privileges and enter the netstat -abno command, as shown in the command output.

![Screenshot (723)](https://github.com/user-attachments/assets/7b6c2696-84a7-47e1-a324-3b90a9448ca7)

Note: If you are not in administrator mode, a “The requested operation requires elevation” message will appear. Search for Command Prompt. Right-click on Command Prompt and chose Run as administrator.

By examining the active TCP connections, an analyst should be able to determine if there are any suspicious programs that are listening for incoming connections on the host. You can also trace that process to the Windows Task Manager and cancel the process. There may be more than one process listed with the same name. If this is the case, use the PID to find the correct process. Each process running on the computer has a unique PID. To display the PIDs for the processes in the Task Manager, open the Task Manager, right-click the table heading and select PID.

# 1.4.2 Event Viewer

Windows Event Viewer logs the history of application, security, and system events. These log files are a valuable troubleshooting tool because they provide information necessary to identify a problem. To open the Event Viewer, search for it and click the program icon, as shown in the figure.

![f0a59c70-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/bff8cf20-b397-4ebb-a281-64f41371c1e2)

Windows includes two categories of event logs: Windows Logs, and Application and Services Logs. Each of these categories has multiple log types. Events that are displayed in these logs have a level: information, warning, error, or critical. They also have the date and time that the event occurred, along with the source of the event and an ID which relates to that type of event.

It is also possible to create a custom view. This is useful when looking for certain types of events, finding events that happened during a certain time period, displaying events of a certain level, and many other criteria. There is a built-in custom view called Administrative Events that shows all critical, error, and warning events from all of the administrative logs. This is a good view to start with when trying to troubleshoot a problem.

Security event logs are found under Windows Logs. They use event IDs to identify the type of event.

# 1.4.3 Windows Update Management

No software is perfect, and the Windows operating system is no exception. Attackers are constantly coming up with new ways to compromise computers and exploit bad code. Some of these attacks come so quickly that defenses against them have not yet been devised and distributed. These are called zero-day exploits. Microsoft and security software developers are always trying to stay ahead of the attackers, but they are not always successful. To ensure the highest level of protection against these attacks, always make sure Windows is up to date with the latest service packs and security patches.

Patches are code updates that manufacturers provide to prevent a newly discovered virus or worm from making a successful attack. From time to time, manufacturers combine patches and upgrades into a comprehensive update application called a service pack. Many devastating virus attacks could have been much less severe if more users had downloaded and installed the latest service pack. It is highly desirable that enterprises utilize systems that automatically distribute, install, and track security updates.

Windows routinely checks the Windows Update website for high-priority updates that can help protect a computer from the latest security threats. These updates include security updates, critical updates, and service packs. Depending on the setting you choose, Windows automatically downloads and installs any high-priority updates that your computer needs or notifies you as these updates become available. To configure the settings for Windows update, search for Windows Update and click the application.

Update status, shown in the figure, allows you to check for updates manually and see the update history of the computer.

![f0a7e660-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/5e64a0aa-4038-4411-9b45-b98e9a4bd883)

There are also settings for the hours where the computer will not automatically restart, for example during regular business hours. You can also choose when to restart the computer after an update, if necessary, with the Restart options. Advanced options are also available to choose how updates are installed how other Microsoft products are updated.

# 1.4.4 Local Security Policy

A security policy is a set of objectives that ensures the security of a network, the data, and the computer systems in an organization. The security policy is a constantly evolving document based on changes in technology, business, and employee requirements.

In most networks that use Windows computers, Active Directory is configured with Domains on a Windows Server. Windows computers join the domain. The administrator configures a Domain Security Policy that applies to all computers that join the domain. Account policies are automatically set when a user logs in to a computer that is a member of a domain. Windows Local Security Policy, shown in the figure, can be used for stand-alone computers that are not part of an Active Directory domain. To open the Local Security Policy applet, search for Local Security Policy and click the program.

![f0aaa580-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/291817eb-9a62-441a-8334-77b011daaf16)

Password guidelines are an important component of a security policy. Any user that must log on to a computer or connect to a network resource should be required to have a password. Passwords help prevent theft of data and malicious acts. Passwords also help to confirm that the logging of events is valid by ensuring that the user is the person that they say they are. In the Local Security Policy, Password Policy is found under Account Policies and defines the criteria for the passwords for all of the users on the local computer.

Use the Account Lockout Policy in Account Policies to prevent brute-force login attempts. For example, you can set the policy to allow the user to enter a wrong username and/or password five times. After five attempts, the account is locked for 30 minutes. After 30 minutes, the number of attempts is reset to zero and the user can attempt to login again.

It is important to make sure that computers are secure when users are away. A security policy should contain a rule about requiring a computer to lock when the screensaver starts. This will ensure that after a short time away from the computer, the screen saver will start and then the computer cannot be used until the user logs in.

If the Local Security Policy on every stand-alone computer is the same, then use the Export Policy feature. Save the policy with a name, such as workstation.inf. Copy the policy file to an external media or network drive to use on other stand-alone computers. This is particularly helpful if the administrator needs to configure extensive local policies for user rights and security options.

The Local Security Policy applet contains many other security settings that apply specifically to the local computer. You can configure User Rights, Firewall Rules, and even the ability to restrict the files that users or groups are allowed to run with the AppLocker.

# 1.4.5 Windows Defender

Malware includes viruses, worms, Trojan horses, keyloggers, spyware, and adware. These are designed to invade privacy, steal information, damage the computer, or corrupt data. It is important that you protect computers and mobile devices using reputable antimalware software. The following types of antimalware programs are available:

- **Antivirus Protection:**
  This program continuously monitors for viruses. When a virus is detected, the user is warned, and the program attempts to quarantine or delete the virus.
- **Adware Protection:**
  This program continuously looks for programs that display advertising on your computer.
- **Phising Protection:**
  This program blocks the IP addresses of known phishing websites and warns the user about suspicious sites.
- **Spyware Protection:**
  This program scans for keyloggers and other spyware.
- **Trusted / untrusted Source:**
  This program warns you about unsafe programs about to be installed or unsafe websites before they are visited.

It may take several different programs and multiple scans to completely remove all malicious software. Run only one malware protection program at a time.

Several reputable security organizations such as McAfee, Symantec, and Kaspersky offer all-inclusive malware protection for computers and mobile devices. Windows has built-in virus and spyware protection called Windows Defender, as shown in the figure. Windows Defender is turned on by default to provide real-time protection against infection.

![f2476590-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/8b39ce61-5f77-4d93-b21c-b8bb4ccbc392)

To open Windows Defender, search for it and click the program. Although Windows Defender works in the background, you can perform manual scans of the computer and storage devices. You can also manually update the virus and spyware definitions in the Update tab. Also, to see all of the items that were found during previous scans, click the History tab.

# 1.4.6 Windows Defender Firewall

A firewall selectively denies traffic to a computer or network segment. Firewalls generally work by opening and closing the ports used by various applications. By opening only the required ports on a firewall, you are implementing a restrictive security policy. Any packet not explicitly permitted is denied. In contrast, a permissive security policy permits access through all ports, except those explicitly denied. In the past, software and hardware were shipped with permissive settings. As users neglected to configure their equipment, the default permissive settings left many devices exposed to attackers. Most devices now ship with settings as restrictive as possible, while still allowing easy setup.

To allow program access through the Windows Defender Firewall, search for **Control Panels**. Under **Systems and Security**, locate **Windows Defender Firewall**. Click **Allow an app or feature through Windows Defender Firewall**, as shown in the figure.

If you wish to use a different software firewall, you will need to disable Windows Firewall. To disable the Windows Firewall, click **Turn Windows Firewall on or off.**

Many additional settings can be found under **Advanced settings. Here you can create inbound or outbound traffic rules based on different criteria. You can also import and export policies or monitor different aspects of the firewall.**

![f35ef010-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/125319ea-8d2a-4803-8953-441bcbd273b4)

