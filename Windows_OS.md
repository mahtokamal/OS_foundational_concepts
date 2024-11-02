# 1.0. Windows Background & Versions History
    Windows Operating System first launched around 35 years ago in 1985. Since then, many versions and editions are released as per
    requirements or business need. For example - from Windows 1.0 to today's Windows desktop versions 11 and Windows Server version
    2019.
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

**Partition Boot Sector** - This is the first 16 sectors of the drive. It contains the location of the Master File Table (MFT). The last 16 sectors contain a copy of the boot sector.
**Master File Table (MFT)** - This table contains the locations of all the files and directories on the partition, including file attributes such as security information and timestamps.
**System Files** - These are hidden files that store information about other volumes and file attributes.
**File Area** - The main area of the partition where files and directories are stored.
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

2. Boot
Any installed operating system can be chosen here to start. There are also options for Safe boot, which is used to troubleshoot startup.

3. Services
All the installed services are listed here so that they can be chosen to start at startup.

4. Startup
All the applications and services that are configured to automatically begin at startup can be enabled or disabled by opening the task manager from this tab.

5. Tools
   Many common operating system tools can be launched directly from this tab.

# 1.2.7 Windows Shutdown
# 1.2.8 Processes, Threads, and Services
# 1.2.9 Memory Allocation and Handles
# 1.2.10 The Windows Registry

# 1.3. Windows Configurations and Monitoring

# 1.4. Windows Security


