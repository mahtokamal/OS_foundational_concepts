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
# 1.2.9 Memory Allocation and Handles
A computer works by storing instructions in RAM until the CPU processes them. The virtual address space for a process is the set of virtual addresses that the process can use. The virtual address is not the actual physical location in memory, but an entry in a page table that is used to translate the virtual address into the physical address.

Each process in a 32-bit Windows computer supports a virtual address space that enables addressing up to 4 gigabytes. Each process in a 64-bit Windows computer supports a virtual address space of 8 terabytes.

Each user space process runs in a private address space, separate from other user space processes. When the user space process needs to access kernel resources, it must use a process handle. This is because the user space process is not allowed to directly access these kernel resources. The process handle provides the access needed by the user space process without a direct connection to it.

A powerful tool for viewing memory allocation is RAMMap, which is shown in the figure. RAMMap is part of the Windows Sysinternals Suite of tools. It can be downloaded from Microsoft. RAMMap provides a wealth of information regarding how Windows has allocated system memory to the kernel, processes, drivers, and applications.
![Screenshot (714)](https://github.com/user-attachments/assets/9b14f4e7-0efb-4b37-836c-4d275f7530c2)

# 1.2.10 The Windows Registry

# 1.3. Windows Configurations and Monitoring

# 1.4. Windows Security




