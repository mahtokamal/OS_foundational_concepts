# 1.0 Introduction

Linux is an open-source operating system that is fast, powerful, and highly customizable. It is built for network use as either a client or server. Linux is well-loved by a large community of users, including cybersecurity personnel.

# 1.1 Linux Basics
# 1.1.1 What is Linux ?

![f47e42c0-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/f0294ec4-558d-46ee-a9c0-4ed89db8ff05)


Linux is an operating system that was created in 1991. Linux is open source, fast, reliable, and small. It requires very little hardware resources to run and is highly customizable. Unlike other operating systems such as Windows and Mac OS X, Linux was created, and is currently maintained by, a community of programmers. Linux is part of several platforms and can be found on devices anywhere from “wristwatches to supercomputers”.

Another important aspect of Linux is that it is designed to be connected to the network, which makes it much simpler to write and use network-based applications. Because Linux is open source, any person or company can get the kernel’s source code, inspect it, modify it, and re-compile it at will. They are also allowed to redistribute the program with or without charges.

A Linux distribution is the term used to describe packages created by different organizations. Linux distributions (or distros) include the Linux kernel with customized tools and software packages. While some of these organizations may charge for their Linux distribution support (geared towards Linux-based businesses), the majority of them also offer their distribution for free without support. Debian, Red Hat, Ubuntu, CentOS, and SUSE are just a few examples of Linux distributions.

# 1.1.2 The Value of Linux

Linux is often the operating system of choice in the Security Operations Center (SOC). These are some of the reasons to choose Linux:

- Linux is open source - Any person can acquire Linux at no charge and modify it to fit specific needs. This flexibility allows analysts and administrators to tailor-build an operating system specifically for security analysis.

- The Linux CLI is very powerful - While a GUI makes many tasks easier to perform, it adds complexity and requires more computer resources to run. The Linux Command Line Interface (CLI) is extremely powerful and enables analysts to perform tasks not only directly on a terminal, but also remotely.

- The user has more control over the OS - The administrator user in Linux, known as the root user, or superuser, has absolute power over the computer. Unlike other operating systems, the root user can modify any aspect of the computer with a few keystrokes. This ability is especially valuable when working with low level functions such as the network stack. It allows the root user to have precise control over the way network packets are handled by the operating system.

- It allows for better network communication control - Control is an inherent part of Linux. Because the OS can be adjusted in practically every aspect, it is a great platform for creating network applications. This is the same reason that many great network-based software tools are available for Linux only.

# 1.1.3 Linux in the SOC

The flexibility provided by Linux is a great feature for the SOC. The entire operating system can be tailored to become the perfect security analysis platform. For example, administrators can add only the necessary packages to the OS, making it lean and efficient. Specific software tools can be installed and configured to work in conjunction, allowing administrators to build a customized computer that fits perfectly in the workflow of a SOC.

The figure shows Sguil, which is the cybersecurity analyst console in a special version of Linux called Security Onion. Security Onion is an open source suite of tools that work together for network security analysis.

![f59027f0-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/625423cd-b0e0-47b9-896e-616a8962106b)

- Network Packet Capture Software
  A crucial tool for a SOC analyst as it makes it possible to observe and understand every detail of a network transaction.

  Wireshark is a popular packet capture tool.

- Malware analysis Tools
  These tools allow analysts to safely run and observe malware execution without the risk of compromising the underlying 
  system.

- Intrusion Detection System (IDSs)
  These tools are used for real-time traffic monitoring and inspection.
  If any aspect of the currently flowing traffic matches any of the established rules, a pre-defined action is taken.

- Firewalls
  This software is used to specify, based on pre-defined rules, whether traffic is allowed to enter or leave a network or 
  device.

- Log Managers
  Log files are used to record events.
  
  Because a network can generate a very large number of log entries, log manager software is employed to facilitate log 
  monitoring.

- Security information and event management (SIEM)
  SIEMs provide real-time analysis of alerts and log entries generated by network appliances such as IDSs and firewalls.

- Ticketing Systems
  Task ticket assignment, editing, and recording is done through a ticket management system. Security alerts are often 
  assigned to analysts through a ticketing system.

# 1.1.4 Linux Tools

In addition to SOC-specific tools, Linux computers that are used in the SOC often contain penetration testing tools. Also known as PenTesting, a penetration test is the process of looking for vulnerabilities in a network or computer by attacking it. Packet generators, port scanners, and proof-of-concept exploits are examples of PenTesting tools.

Kali Linux is a Linux distribution groups many penetration tools together in a single Linux distribution. Kali contains a great selection of tools. The figure shows a screenshot of Kali Linux. Notice all the major categories of penetration testing tools.

![f59298f0-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/026a9300-deef-4e67-b582-ee97fd9667c9)


# 1.2 Working in the Linux Shell
# 1.2.1 The Linux Shell

In Linux, the user communicates with the OS by using the CLI or the GUI. Linux often starts in the GUI by default. This hides the CLI from the user. One way to access the CLI from the GUI is through a terminal emulator application. These applications provide user access to the CLI and are often named as some variation of the word “terminal”. In Linux, popular terminal emulators are Terminator, eterm, xterm, konsole, and gnome-terminal.

Fabrice Bellard has created JSLinux which allows an emulated version of Linux to run in a browser. Search for it on the internet. Open a Linux console in JSLinux and type the ls command to list the current directory content. Keep the tab open if you would like to try out some of the other commands discussed in this chapter.

The figure shows gnome-terminal, a popular Linux terminal emulator.

Note: The terms shell, console, console window, CLI terminal, and terminal window are often used interchangeably.

![f59446a0-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/2c8a6fdd-f527-4b41-98f7-f4139ddb41b1)

# 1.2.2 Basic Commands

Linux commands are programs created to perform a specific task. Use the man command (short for manual) to obtain documentation about commands. As an example, man Is provides documentation about the Is command from the user manual.

Because commands are programs stored on the disk, when a user types a command, the shell must find it on the disk before it can be executed. The shell will look for user-typed commands in specific directories and attempt to execute them. The list of directories checked by the shell is called the path. The path contains many directories commonly used to store commands. If a command is not in the path, the user must specify its location, or the shell will not be able to find it. Users can easily add directories to the path, if necessary.

To invoke a command via the shell, simply type its name. The shell will try to find it in the system path and execute it.

The table lists basic Linux commands and their functions.

|Command|Description|
--------|-----------|
|mv||
|chmod||
|chown||
|dd||
|pwd||
|ps||
|su||
|sudo||
|grep||
|ifconfig||
|apt-get||
|iwconfig||
|shutdown||
|passwd||
|cat||
|man||

# 1.2.3 File and Directory Commands

Many command line tools are included in Linux by default. To adjust the command operation, users can pass parameters and switches along with the command. The table lists a few of the most common commands related to files and directories.

|Command|Description|
--------|-----------|
|ls||
|cd||
|mkdir||
|cp||
|mv||
|rm||
|grep||
|cat||

# 1.2.4 Working with Text Files

Linux has many different text editors, with various features and functions. Some text editors include graphical interfaces while others are command-line only tools. Each text editor includes a feature set designed to support a specific type of task. Some text editors focus on the programmer and include features such as syntax highlighting, brackets and parenthesis check, and other programming-focused features.

While graphical text editors are convenient and easy to use, command line-based text editors are very important for Linux users. The main benefit of command-line-based text editors is that they allow for text file editing from a remote computer.

Consider the following scenario: a user must perform administrative tasks on a Linux computer but is not sitting in front of that computer. Using SSH, the user starts a remote shell to the remote computer. Under the text-based remote shell, the graphical interface is not available, which makes it impossible to rely on tools such as graphical text editors. In this type of situation, text-based programs are crucial.

The figure shows nano, a popular command-line text editor. The administrator is editing firewall rules. Text editors are often used for system configuration and maintenance in Linux.

![f68a6670-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/c5b15602-e3ad-42a8-a397-023e263bba98)

Due to the lack of graphical support, nano (or GNU nano) can only be controlled with the keyboard. For example, CTRL+O saves the current file; CTRL+W opens the search menu. GNU nano uses a two-line shortcut bar at the bottom of the screen, where commands for the current context are listed. Press CTRL+G for the help screen and a complete list of commands.

# 1.2.5 The Importance of Text Files in Linux

In Linux, everything is treated as a file. This includes the memory, the disks, the monitor, and the directories. For example, from the operating system standpoint, showing information on the display means to write to the file that represents the display device. It should be no surprise that the computer itself is configured through files. Known as configuration files, they are usually text files used to store adjustments and settings for specific applications or services. Practically everything in Linux relies on configuration files to work. Some services have not one, but several configuration files.

Users with proper permission levels can use text editors to change the contents of configuration files. After the changes are made, the file is saved and can be used by the related service or application. Users are able to specify exactly how they want any given application or service to behave. When launched, services and applications check the contents of specific configuration files to adjust their behavior accordingly.

In the figure, the administrator opened the host configuration file in nano for editing. The host file contains static mappings of host IP addresses to names. The names serve as shortcuts that allow connecting to other devices by using a name instead of an IP address. Only the superuser can change the host file.

Note: The administrator used the command sudo nano /etc/hosts to open the file. The command sudo (short for “superuser do”) invokes the superuser privilege to use the nano text editor to open the host file.

![f77821d0-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/009aa52e-9ff9-4205-9619-7a0cc9d2a661)

# 1.3 Linux Servers and Clients
# 1.3.1 An Introduction to Client-Server Communications

Servers are computers with software installed that enables them to provide services to clients across the network. There are many types of services. Some provide external resources such as files, email messages, or web pages to clients upon request. Other services run maintenance tasks such as log management, memory management, disk scanning, and more. Each service requires separate server software. For example, the server in the figure uses file server software to provide clients with the ability to retrieve and submit files.

![Screenshot (727)](https://github.com/user-attachments/assets/5c0a85a6-740d-4630-bb81-07c02b0f2d4c)

# 1.3.2 Servers, Services, and Their Ports
In order that a computer can be the server for multiple services, ports are used. A port is a reserved network resource used by a service. A server is said to be "listening" on a port when it has associated itself to that port.

While the administrator can decide which port to use with any given service, many clients are configured to use a specific port by default. It is common practice to leave the service running in its default port. The table lists a few commonly used ports and their services. These are also called "well-known ports".

| Ports| Description|
-------|------------|
|20/21|FTP|
|22|SSH|
|23|Telnet|
|25|SMTP|
|53|DNS|
|67/68|DHCP|
|69|TFTP|
|80|HTTP|
|110|POP3|
|123|NTP|
|143|IMAP|
|161/162|SNMP|
|443|HTTPS|
# 1.3.3 Clients
Clients are programs or applications designed to communicate with a specific type of server. Also known as client applications, clients use a well-defined protocol to communicate with the server. Web browsers are web clients that are used to communicate with web servers through the Hyper Text Transfer Protocol (HTTP) on port 80. The File Transfer Protocol (FTP) client is software used to communicate with an FTP server. The figure shows a client uploading files to a server.

![Screenshot (728)](https://github.com/user-attachments/assets/8df9d77b-ec99-4a20-b74a-c1dbd6e3e599)

# 1.3.4
# 1.3.5

# 1.4 Basic Server Administration
# 1.4.1 Service Configuration Files

In Linux, services are managed using configuration files. Common options in configuration files are port number, location of the hosted resources, and client authorization details. When the service starts, it looks for its configuration files, loads them into memory, and adjusts itself according to the settings in the files. Configuration file modifications often require restarting the service before the changes take effect.

Because services often require superuser privileges to run, service configuration files often require superuser privileges to edit.

The command output shows a portion of the configuration file for Nginx, which is a lightweight web server for Linux.

![Screenshot (729)](https://github.com/user-attachments/assets/5120df8d-b9e9-4fc2-aadb-bed3ea08b5fa)

The next command output shows the configuration file for the network time protocol (NTP).

![Screenshot (730)](https://github.com/user-attachments/assets/460bade3-722d-4e11-9e4e-e99d0f556b0b)

The last command output shows the configuration file for Snort, a Linux-based intrusion detection system (IDS).

![Screenshot (731)](https://github.com/user-attachments/assets/cf7dffba-4ce5-4f9b-8f37-be82afad0018)

There is no rule for a configuration file format; it is the choice of the service’s developer. However, the option = value format is often used. For example, in the last command output, the variable ipvar is configured with several options. The first option, HOME_NET, has the value 209.165.200.224/27. The hash character (#) is used to indicate comments.


# 1.4.2 Hardening Devices

Device hardening involves implementing proven methods of securing the device and protecting its administrative access. Some of these methods involve maintaining passwords, configuring enhanced remote login features, and implementing secure login with SSH. Defining administrative roles in terms of access is another important aspect of securing infrastructure devices because not all information technology personnel should have the same level of access to the infrastructure devices.

Depending on the Linux distribution, many services are enabled by default. Some of these features are enabled for historical reasons but are no longer required. Stopping such services and ensuring they do not automatically start at boot time is another device hardening technique.

OS updates are also extremely important to maintaining a hardened device. New vulnerabilities are discovered every day. OS developers create and issue fixes and patches regularly. An up-to-date computer is less likely to be compromised.

The following are basic best practices for device hardening.

- Ensure physical security
- Minimize installed packages
- Disable unused services
- Use SSH and disable the root account login over SSH
- Keep the system updated
- Disable USB auto-detection
- Enforce strong passwords
- Force periodic password changes
- Keep users from re-using old passwords

Many other steps exist and are often service or application-dependent.


# 1.4.3 Monitoring Service Logs

Log files are the records that a computer stores to keep track of important events. Kernel, services, and application events are all recorded in log files. It is very important for an administrator to periodically review the logs of a computer to keep it healthy. By monitoring Linux log files, an administrator gains a clear picture of the computer's performance, security status, and any underlying issues. Log file analysis allows an administrator to guard against upcoming issues before they occur.

In Linux, log files can be categorized as:
- Application logs
- Event logs
- Service logs
- System logs

Some logs contain information about daemons that are running in the Linux system. A daemon is a background process that runs without the need for user interaction. For example, the System Security Services Daemon (SSSD) manages remote access and authentication for single sign-on capabilities.

The table lists a few popular Linux log files and their functions.

|Linux Log File|Description|
|--------------|-----------|
|/var/log/messages|- This directory contains generic computer activity logs. <br> - It is mainly used to store informational and non-critical system messages. <br> - In Debian-based computers, /var/log/syslog directory serves the same purpose.|
|/var/log/auth.log|- This file stores all authentication - related events in Debian and Ubuntu computers. <br> - Anything involving the user authorization mechanism can be found in this file.|
|/var/log/secure|- This directory is used by RedHat and CentOS computers instead of /var/log/auth.log. <br> - It also tracks sudo logins, SSH logins, and other errors logged by SSSD.|
|/var/log/boot.log|- This file stores boot-related information and messages logged during the computer startup process.|
|/var/log/dmesg|- This directory contains kernel ring buffer messages. <br> - Information realted to hardware devices and their driver is recorded here. <br> - It is very important because, due to their low-level nature, logging systems such as syslog are not running when these events take place and therefore are often unavailable to the administrator in real-time.|
|/var/log/kern.log||
|/var/log/cron||
|/var/log/mysqld.log or /var/log/mysql.log ||

The command output shows a portion of **/var/log/messages** log file. Each line represents a logged event. The timestamps at the beginning of the lines mark the moment the event took place.

![Screenshot (732)](https://github.com/user-attachments/assets/18251146-bc3a-451e-a4cc-30c1ff3c19c0)

# 1.4.4 Lab - Locating Log Files

In this lab, you will get familiar with locating and manipulating Linux log files.

- Part 1: Log File Overview
- Part 2: Locating Log Files in Unknown Systems
- Part 3: Monitoring Log Files in Real Time

# 1.5 The Linux File System
# 1.5.1 The File System Types in Linux

There are many different kinds of file systems, varying in properties of speed, flexibility, security, size, structure, logic and more. It is up to the administrator to decide which file system type best suits the operating system and the files it will store.

**1. ext2 (second extended file system)**

- ext2 was the default file system in several major Linux distributions until supplanted by ext3.
- Almost fully compatible with ext2, ext3 also supports journaling (see below).
- ext2 is still the file system of choice for flash-based storage media because its lack of a journal increases performance and minimizes the number of writes.
- Because flash memory devices have a limited number of write operations, minimizing write operations increases the device’s lifetime.
- However, contemporary Linux kernels also support ext4, an even more modern file system, with better performance and which can also operate in a journal-less mode.

**2. ext3 (third extended file system)**

- ext3 is a journaled file system designed to improve the existing ext2 file system.
- A journal, the main feature added to ext3, is a technique used to minimize the risk of file system corruption in the event of sudden power loss.
- The file systems keeps a log (or journal) of all the file system changes about to be made.
- If the computer crashes before the change is complete, the journal can be used to restore or correct any eventual issues created by the crash.
- The maximum file size in ext3 file systems is 32 TB.

**3. ext4 (fourth extended file system)**

- Designed as a successor of ext3, ext4 was created based on a series of extensions to ext3.
- While the extensions improve the performance of ext3 and increase supported file sizes, Linux kernel developers were concerned about stability issues and were opposed to adding the extensions to the stable ext3.
- The ext3 project was split in two; one kept as ext3 and its normal development and the other, named ext4, incorporated the mentioned extensions.

**4. NFS (Network Files System)**

- NFS is a network-based file system, allowing file access over the network.
- From the user standpoint, there is no difference between accessing a file stored locally or on another computer on the network.
- NFS is an open standard which allows anyone to implement it.

**5. CDFS (Compact Disc File System)**

CDFS was created specifically for optical disk media.

**6. Swap File System**

- The swap file system is used by Linux when it runs out of RAM.
- Technically, it is a swap partition that does not have a specific file system, but it is relevant to the file system discussion.
- When this happens, the kernel moves inactive RAM content to the swap partition on the disk.
- While swap partitions (also known as swap space) can be useful to Linux computers with a limited amount of memory, they should not be considered as a primary solution.
- Swap partition is stored on disk which has much lower access speeds than RAM.

**7. HFS Plus or HFS+ (Hierarchical File System Plus)**

- A file system used by Apple in its Macintosh computers.
- The Linux kernel includes a module for mounting HFS+ for read-write operations.

**8. APFS (Apple File System)**

An updated file system that is used by Apple devices. It provides strong encryption and is optimized for flash and solid-state drives.

**9. MBR (Master Boot Record)**

- Located in the first sector of a partitioned computer, the MBR stores all the information about the way in which the file system is organized.
- The MBR quickly hands over control to a loading function, which loads the OS.

Mounting is the term used for the process of assigning a directory to a partition. After a successful mount operation, the file system contained on the partition is accessible through the specified directory. In this context, the directory is called the mounting point for that file system. Windows users may be familiar with a similar concept: the drive letter.

The command output shows the output of the **mount** command issued in the Cisco CyberOPS VM.

![Screenshot (733)](https://github.com/user-attachments/assets/f9d780b0-218f-415e-bb7c-5a702f54a906)

When issued with no options, **mount** returns the list of file systems currently mounted in a Linux computer. While many of the file systems shown are out of the scope of this course, notice the root file system (highlighted). The root file system is represented by the “/” symbol and holds all files in the computer by default. It is also shown in the output that the root file system was formatted as ext4 and occupies the first partition of the first drive (/dev/sda1).

# 1.5.2 Linux Roles and File Permissions

In Linux, most system entities are treated as files. In order to organize the system and enforce boundaries within the computer, Linux uses file permissions. File permissions are built into the file system structure and provide a mechanism to define permissions on every file. Every file in Linux carries its file permissions, which define the actions that the owner, the group, and others can perform with the file. The possible permission rights are Read, Write and Execute. The ls command with the -l parameter lists additional information about the file.

Consider the output of the ls -l command in the command output.

![Screenshot (734)](https://github.com/user-attachments/assets/1d8a09f8-8aef-405e-81e2-80fb3c372bc5)

The output provides a lot of information about the file space.txt.

The first field of the output displays the permissions that are associated with **space.txt (-rwxrw-r--).** File permissions are always displayed in the User, Group, and Other order.

The file **space.txt** in has the following permissions:

- The dash (-) means that this is a file. For directories, the first dash would be a “d”.
- The first set of characters is for user permission (rwx ). The user, analyst, who owns the file can Read, Write and eXecute the file.
- The second set of characters is for group permissions (rw-). The group, staff, who owns the file can Read and Write to the file.
- The third set of characters is for any other user or group permissions (r--). Any other user or group on the computer can only Read the file.

The second field defines the number of hard links to the file (the number 1 after the permissions). A hard link creates another file with a different name linked to the same place in the file system (called an inode). This is in contrast to a symbolic link, which is discussed on the next page.

The third and fourth field display the user (**analyst**) and group (**staff**) who own the file, respectively.

The fifth field displays the file size in bytes. The **space.txt** file has 253 bytes.

The sixth field displays the date and time of the last modification.

The seventh field displays the file name.

The figure shows a breakdown of file permissions in Linux.

![Screenshot (735)](https://github.com/user-attachments/assets/2de6d8be-ee4b-4793-af10-334bbed809f5)

Use octal values to define permissions.

|Binary|Octal|Permission|Description|
|-------|-----|------|-----|
|000|0|---|No Access|
|001|1|--x|Execute only|
|010|2|-w-|Write only|
|011|3|-wx|Write and Execute |
|100|4|r--|Read only|
|101|5|r-x|Read and Execute|
|110|6|rw-|Read and Write|
|111|7|rwx|Read, Write and Execute|

File permissions are a fundamental part of Linux and cannot be broken. A user has only the rights to a file that the file permissions allow. The only user that can override file permission on a Linux computer is the root user. Because the root user has the power to override file permissions, the root user can write to any file. Because everything is treated as a file, the root user has full control over a Linux computer. Root access is often required before performing maintenance and administrative tasks. Because of the power of the root user, root credentials should use strong passwords and not be shared with anyone other than system administrators and other high-level users.

# 1.5.3 Hard Links and Symbolic Links

A hard link is another file that points to the same location as the original file. Use the command ln to create a hard link. The first argument is the existing file and the second argument is the new file. As shown in the command output, the file **space.txt** is linked to **space.hard.txt** and the link field now shows 2.

![Screenshot (736)](https://github.com/user-attachments/assets/90643140-4694-403a-b5f2-1806ff4c29a3)

Both files point to the same location in the file system. If you change one file, the other is changed, as well. The **echo** command is used to add some text to **space.txt.** Notice that the file size for both **space.txt** and **space.hard.txt** increased to 257 bytes. If you delete the space.hard.txt with the rm command (remove), the **space.txt** file still exists, as verified with the **more space.txt** command.

A symbolic link, also called a symlink or soft link, is similar to a hard link in that applying changes to the symbolic link will also change the original file. As shown in the command output below, use the **ln** command option **-s** to create a symbolic link.

![Screenshot (737)](https://github.com/user-attachments/assets/2f8488c6-afb2-470c-9090-fb29b489a582)

Notice that adding a line of text to **test.txt** also adds the line to **mytest.txt**. However, unlike a hard link, deleting the original text.txt file means that **mytext.txt** is now linked to a file that no longer exists, as shown with the more **mytest.txt** and **ls -l mytest.txt**commands.

Although symbolic links have a single point of failure (the underlying file), symbolic links have several benefits over hard links:

- Locating hard links is more difficult. Symbolic links show the location of the original file in the ls -l command, as shown in the last line of output in the previous command output **(mytest.txt -> test.txt)**.
- Hard links are limited to the file system in which they are created. Symbolic links can link to a file in another file system.
- Hard links cannot link to a directory because the system itself uses hard links to define the hierarchy of the directory structure. However, symbolic links can link to directories.

# 1.5.4 Lab - Navigating the Linux Filesystem and Permission Settings

# 1.6 Working with GUI
# 1.6.1 X Window System

The graphical interface present in most Linux computers is based on the X Window System. Also known as X or X11, X Window is a windowing system designed to provide the basic framework for a GUI. X includes functions for drawing and moving windows on the display device and interacting with a mouse and keyboard.

X works as a server which allows a remote user to use the network to connect, start a graphical application, and have the graphical window open on the remote terminal. While the application itself runs on the server, the graphical aspect of it is sent by X over the network and displayed on the remote computer.

Notice that X does not specify the user interface, leaving it to other programs, such as window managers, to define all the graphical components. This abstraction allows for great flexibility and customization as graphical components such as buttons, fonts, icons, window borders, and color schemes are all defined by the user application. Because of this separation, the Linux GUI varies greatly from distribution to distribution. Examples of window managers are Gnome and KDE. While the look and feel of window managers vary, the main components are still present.

The figure displays the Gnome Window Manager.

![f78a9860-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/1e26fb4f-a741-41c8-9590-9d9b32aab4f2)

This figure displays the KDE Windows Manager.

![f78bf7f0-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/312eb6f5-58eb-42ee-b776-297d56ec02bb)

# 1.5.4 Lab - Navigating the Linux Filesystem and Permission Settings

# 1.6.2 The Linux GUI

Although an operating system does not require a GUI to function, GUIs are considered more user-friendly than the CLI. The Linux GUI as a whole can be easily replaced by the user. As a result of the large number of Linux distributions, this module focuses on Ubuntu when covering Linux because it is a very popular and user-friendly distribution.

Ubuntu Linux uses Gnome 3 as its default GUI. The goal of Gnome 3 is to make Ubuntu even more user-friendly. The table lists the main UI components of Unity.

The figure shows the location of some of the features of the Ubuntu Gnome 3 Desktop.

![f8a15f90-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/c9288e7d-3f12-4841-94c0-65bd736682ae)

|UI Component|Description|
|------------|-----------|
|Apps Menu|- The Apps Menu shows icons for the apps that are installed on the system.<br> - A right-click menu provides shortcuts that allow starting or configuring the apps.<br>  - The system search box is available from Activities View.|
|Ubuntu Doc|- This is a dock on the left side of the screen that serves as an application launcher and switcher for app favorites.<br> - Click to launch an application and when the application is running, click again to switch between running applications.<br> - If more than one instance of an application is running, Launcher will display all instances.<br> - Right-click any application that is hosted on the launcher to see details about that the application.|
|Top Bar|- This multipurpose menu bar contains a menu for the application that currently has the focus.<br> - It displays the current time and indicates whether there are new system messages.<br> - It also provides access to the Activity desktop view and the system Status Menu.|
|Calendar and System Message Tray| - Click the day and time to see the full appointment calendar and any current system messages.<br> - Access the appointment calendar from here to create new appointments.|
|Activities|- Switch to application view to switch to or close running applications.<br> - A powerful search tool is available here that will find apps, files, and values within files.<br> - Allows switching between workspaces.|
|Status Menu|- Allows configuration of the network adaptor and other running devices.<br> - The current user can logoff or change their settings.<br> - System configuration changes can be made here.<br> - The workstation can be locked or shutdown from here.|

# 1.7 Working on a Linux Host
# 1.7.1 Installing and Running Applications on a Linux Host

Many end-user applications are complex programs written in compiled languages. To aid in the installation process, Linux often includes programs called package managers. A package is the term used to refer to a program and all its supporting files. By using a package manager to install a package, all the necessary files are placed in the correct file system location.

Package managers vary depending on Linux distributions. For example, **pacman** is used by Arch Linux while **dpkg** (Debian package) and **apt** (Advanced Packaging Tool) are used in Debian and Ubuntu Linux distributions.

The command output shows the output of a few **apt-get** commands used in Debian distributions.

![Screenshot (738)](https://github.com/user-attachments/assets/4f97c145-7666-49a2-9377-b82a3808c7ca)

The **apt-get update** command is used to get the package list from the package repository and update the local package database. The **apt-get upgrade** command is used to update all currently installed packages to their latest versions.

# 1.7.2 Keeping the System Up to Date

Also known as patches, OS updates are released periodically by OS companies to address any known vulnerabilities in their operating systems. While companies have update schedules, the release of unscheduled OS updates can happen when a major vulnerability is found in the OS code. Modern operating systems will alert the user when updates are available for download and installation, but the user can check for updates at any time.

The following table compares Arch Linux and Debian / Ubuntu Linux distribution commands to perform package system basic operations.

|Task|Arch|Debian / Ubuntu|
|-----|--|--|
|Install a package by name |pacman -S |apt install|
|Remove a package by name |pacman -Rs|apt remove|
|Update a local package|pacman -Syy|apt-get update|
|Upgrade all currently installed packages |pacman -Syu|apt-get upgrade|

A Linux GUI can also be used to manually check and install updates. In Ubuntu for example, to install updates you would click **Dash Search Box** , type **software updater** , and then click the **Software Updater** icon, as shown in the figure.

![f8a4baf0-a1fb-11ea-bb42-49e522ad4be8](https://github.com/user-attachments/assets/a77a973e-cfed-46f8-a4ce-e8cfc2d7516c)

# 1.7.3 Processes and Forks

A process is a running instance of a computer program. Multitasking operating systems can execute many processes at the same time.

Forking is a method that the kernel uses to allow a process to create a copy of itself. Processes need a way to create new processes in multitasking operating systems. The fork operation is the only way of doing so in Linux.

Forking is important for many reasons. One of them relates to process scalability. Apache, a popular web server, is a good example. By forking itself, Apache is able to serve a large number of requests with fewer system resources than a single-process-based server.

When a process calls a fork, the caller process becomes the parent process, with the newly created process referred to as its child. After the fork, the processes are, to some extent, independent processes; they have different process IDs but run the same program code.

The table lists three commands that are used to manage processes.

|Command|Description|
|------|------|
|ps|- Used to list the processes running on the computer at the time it is invoked. <br> - It can be instructed to display running processes that belong to the current user or other users. <br> - While listing processes does not require root privileges, killing or modifying other user's processes does.|
|top|- Used to list running processes, but unlike ps, top keeps displaying running processes dynamically. <br> - Press q to exit top.|
|kill|- Used to modify the behavior of a specific process. <br> - Depending on the parameters, kill will remove, restart, or pause a process. <br> - In many cases, the user will run ps or top before running kill.<br> - This is done so the user can learn the PID of a process before running kill.|

The command output shows the output of the top command on a Linux computer.
![Screenshot (740)](https://github.com/user-attachments/assets/9fe6efb0-2ff1-43da-9a9b-9a7d52078c18)

# 1.7.4 Malware on a Linux Host

Linux malware includes viruses, Trojan horses, worms, and other types of malware that can affect the operating system. Due to a number of design components such as file system structure, file permissions, and user account restrictions, Linux operating systems are generally regarded as better protected against malware.

While arguably better protected, Linux is not immune to malware. Many vulnerabilities have been found and exploited in Linux. These range from server software to kernel vulnerabilities. Attackers are able to exploit these vulnerabilities and compromise the target. Because Linux is open source, fixes and patches are often made available within hours of the discovery of such problems.

If a malicious program is executed, it will cause damage, regardless of the platform. A common Linux attack vector is its services and processes. Vulnerabilities are frequently found in server and process code running on computers connected to the network. An outdated version of the Apache web server could contain an unpatched vulnerability which can be exploited by an attacker, for example. Attackers often probe open ports to assess the version and nature of the server running on that port. With that knowledge, attackers can research if there are any known issues with that particular version of that particular server to support the attack. As with most vulnerabilities, keeping the computer updated and closing any unused services and ports is a good way to reduce the opportunities for attack in a Linux computer.

The command output shows an attacker using the Telnet command to probe the nature and version of a web server (port 80).

![Screenshot (741)](https://github.com/user-attachments/assets/4a107b6f-4e36-4e07-b0a7-aa30b061c4dc)

The attacker has learned that the server in question is running nginx version 1.12.0. The next step would be to research known vulnerabilities in the nginx 1.12.0 code.

# 1.7.5 Rootkit Check

A rootkit is a type of malware that is designed to increase an unauthorized user’s privileges or grant access to portions of the software that should not normally be allowed. Rootkits are also often used to secure a backdoor to a compromised computer.

The installation of a rootkit can be automated (done as part of an infection) or an attacker can manually install it after compromising a computer. A rootkit is destructive because it changes kernel code and its modules, changing the most fundamental operations of the OS itself. With such a deep level of compromise, rootkits can hide the intrusion, remove any installation tracks, and even tamper with troubleshooting and diagnostic tools so that their output now hides the presence of the rootkit. While a few Linux vulnerabilities through history have allowed rootkit installation via regular user accounts, the vast majority of rootkit compromises require root or administrator access.

Because the very nature of the computer is compromised, rootkit detection can be very difficult. Typical detection methods often include booting the computer from trusted media such as a diagnostics operating system live CD. The compromised drive is mounted and, from the trusted system toolset, trusted diagnostic tools can be launched to inspect the compromised file system. Inspection methods include behavioral-based methods, signature scanning, difference scanning, and memory dump analysis.

Rootkit removal can be complicated and often impossible, especially in cases where the rootkit resides in the kernel; re-installation of the operating system is usually the only real solution to the problem. Firmware rootkits usually require hardware replacement.

**chkrootkit** is a popular Linux-based program designed to check the computer for known rootkits. It is a shell script that uses common Linux tools such as **strings** and **grep** to compare the signatures of core programs. It also looks for discrepancies as it traverses the /proc file system comparing the signatures found there with the output of **ps**.

While helpful, keep in mind that programs to check for rootkits are not 100% reliable.

The command output shows the output of chkrootkit on an Ubuntu Linux.

![Screenshot (742)](https://github.com/user-attachments/assets/6794c5bf-7859-46e7-8eab-5f2e75f09b8d)

# 1.7.6 Piping Commands

Although command line tools are usually designed to perform a specific, well-defined task, many commands can be combined to perform more complex tasks by a technique known as piping. Named after its defining character, the pipe (|), piping consists of chaining commands together, feeding the output of one command into the input of another.

For example, the ls command is used to display all the files and directories of a given directory. The **grep** command compares searches through a file or text looking for the specified string. If found, **grep** displays the entire contents of the folder where the string was found.

The two commands, **ls** and **grep**, can be piped together to filter out the output of **ls**. This is shown in the output of the **ls -l | grep host** command and the **ls -l | grep** file command.

![Screenshot (743)](https://github.com/user-attachments/assets/d84c31fe-bc34-4bc8-9d44-2063e4711c72)

# 1.7.7 Video - Applications, Rootkits, and Piping Commands
# 1.7.8 Lab - Configure Security Features in Windows and Linux

# 1.8 Linux Overview Summary
# 1.8.1 What did we learn in this module?

1. Linux Basics

   Linux is a fast, reliable, and small open-source operating system. It requires few hardware resources to run and is highly customizable. It is designed to be used on networks. The Linux kernel is distributed by different organizations with different tools and software packages. A customized version of Linux that is called Security Onion contains software and tools that are designed for use in network security monitoring by cybersecurity analysts. Kali Linux is another customized Linux distribution that has numerous tools that are designed for network security penetration testing.
   
3. Working in the Linux Shell

In Linux, the user communicates with the operating system through a GUI or a command-line interface (CLI), or shell. If a GUI is running, the shell is accessed through at terminal application such as xterm or gnome terminal. Linux commands are programs that perform a specific task. The man command, followed by a specific command, provides documentation for that command. It is important to know at least basic Linux commands, file and directory commands, and commands for working with text files. In Linux everything is treated is if it were a file, including the memory, disks, monitor, and directories.
   
5. Linux Server and Clients

   Servers are computers that have software installed that enables them to provide services to client computers across the network. Some services provide access to external resources such as files, email, and web pages, to clients upon request. Other services run internally and perform tasks such as log management, memory management, or disk scanning. To enable a computer to provide multiple services, ports are used. A port is a reserved network resource that “listens” for requests by clients. While the port number that is used by a service can be configured, most services listen on default “well-known” ports. Client software applications are designed to communicate with specific types of servers. Web browsers are designed to communicate with web servers by using the HTTP protocol on port 80. FTP clients communicate with FTP servers to transfer files.
   
7. Basic Server Administrations

   In Linux, servers are managed by using configuration files. Various settings can be modified and saved in configuration files. When a service is started, it looks at its configuration file(s) to know how it should run. There is no rule for the way configuration files are written. Configuration file formatting depends on the creator of the server software. Linux devices should be secured by using proven methods to protect the device and administrative access. This is known as hardening devices. One way to harden a device is to maintain passwords, configure enhanced login features, and implement secure remote login with SSH. It is also very important to keep the operating system up to date. Other ways to harden a device are to force periodic password changes, enforce strong passwords, and to prevent reuse of passwords. Finally, Linux clients and servers use logfiles to record the operation of the system and important events. A number of different logfiles are maintained including application logs, event logs, service logs, and system logs. Server logs record activities that are conducted by remote users who access system services. It is important to know the location of different logs in the Linux file system so that they can be accessed and monitored for problems.
   
9. The Linux File System

    Linux supports a number of different file systems that vary by speed, flexibility, security, size, structure, logic, and more. Some of the file systems that are supported by Linux are ext2, ext3, ext4, NFS, and CDFS. File systems are mounted on partitions and accessed through mounting points, or directories. Windows drive letters are examples of mounting points. The mount command can be used to display details of the file systems that are currently mounted on a Linux computer. The root file system is represented by the “/” symbol. It contains all of the files in the computer by default. Linux uses file permissions to control who is permitted to have different types of access to files and directories. Permissions include read (r), write (w), and execute (x). Files and directories have permissions that are assigned for users, groups, and others. The permissions for files and folders are displayed with the ls -l command. This command also displays the links for a file. Hard links create another file with a different name that is linked to the same place in the file system. The owner of the file and the group for the file are also displayed along with the date and time of the last modification to the file. File permissions are powerful features of the Linux file system and can’t be violated. Only the root user can override file permissions. Because of the power of the root user, root access should be carefully controlled. Hard links are created with the ln command. Changes to one of the hard-linked files are also made to the original file. Symbolic links, or symlinks, are similar to hard links in that a change to the linked file is reflected in the original file. Symbolic links have several advantages over hard links.
   
11. working with Linux GUI

    The X Windows, or X11, system is a basic software framework that includes functions for creating, controlling, and configuring a windows GUI in a point-and-click interface. Different vendors use the X Windows system to create different windows manager GUIs for Linux. Examples of windows managers are Gnome and KDE. The Ubuntu Linux distribution uses Gnome 3 by default. The Gnome 3 desktop consists of the Apps Menu, Ubuntu Dock, Top Bar, Calendar and System Message tray, the Activities area, and the Status Menu.
    
13. Working on a Linux Host

In order to install applications on Linux hosts, programs called package managers are used. Packages are software applications and all of their supporting files. Package managers are extremely helpful for installing complex software applications from centralized package repositories that are accessible over the internet. Different Linux distributions use different package managers. For example, Arch Linux uses pacman, Debian uses dpkg as the base package manager and apt to communicate with dpkg. Ubuntu also uses apt. Package manager CLI commands are used to install, remove, and update software packages. Upgrade commands upgrade all currently installed packages. Package management can also be performed in a GUI. Software processes are instances of computer programs that are running. Multitasking operating systems can run many processes at the same time. Forking is a method that the kernel uses to allow a running process to copy itself. The ps command lists the running processes, top displays information about running processes dynamically, and kill is used to remove, restart, or pause running processes. While Linux is considered to be better protected against malicious software (malware) than other operating systems, it is still susceptible to Trojan horses, worms, and other types of malware. Linux is usually attacked through its services and processes. Out of date software is often vulnerable to attack. Threat actors can probe a device for open ports that are linked to out of date server processes. With this knowledge, attacks can be launched. It is important to keep the operating system and its components and applications up to date. The chkrootkit program is designed to detect rootkit malware. Rootkits are deep level malware programs that are very difficult to detect and remove. They can change the fundamental operation of the operating system itself and can be used to create unauthorized access to systems. Piping commands uses the “|” symbol to chain different commands together by using the output of one command as the input for another.

# 1.8 Linux Overview Summary
# 1.8.1 What Did I Learn in this Module?
- Linux Basics
  
Linux is a fast, reliable, and small open-source operating system. It requires few hardware resources to run and is highly customizable. It is designed to be used on networks. The Linux kernel is distributed by different organizations with different tools and software packages. A customized version of Linux that is called Security Onion contains software and tools that are designed for use in network security monitoring by cybersecurity analysts. Kali Linux is another customized Linux distribution that has numerous tools that are designed for network security penetration testing.
  
- Working in the Linux Shell

In Linux, the user communicates with the operating system through a GUI or a command-line interface (CLI), or shell. If a GUI is running, the shell is accessed through at terminal application such as xterm or gnome terminal. Linux commands are programs that perform a specific task. The man command, followed by a specific command, provides documentation for that command. It is important to know at least basic Linux commands, file and directory commands, and commands for working with text files. In Linux everything is treated is if it were a file, including the memory, disks, monitor, and directories.

- Linux Severs and Clients

Servers are computers that have software installed that enables them to provide services to client computers across the network. Some services provide access to external resources such as files, email, and web pages, to clients upon request. Other services run internally and perform tasks such as log management, memory management, or disk scanning. To enable a computer to provide multiple services, ports are used. A port is a reserved network resource that “listens” for requests by clients. While the port number that is used by a service can be configured, most services listen on default “well-known” ports. Client software applications are designed to communicate with specific types of servers. Web browsers are designed to communicate with web servers by using the HTTP protocol on port 80. FTP clients communicate with FTP servers to transfer files.

- Basic Servers Administartion

In Linux, servers are managed by using configuration files. Various settings can be modified and saved in configuration files. When a service is started, it looks at its configuration file(s) to know how it should run. There is no rule for the way configuration files are written. Configuration file formatting depends on the creator of the server software. Linux devices should be secured by using proven methods to protect the device and administrative access. This is known as hardening devices. One way to harden a device is to maintain passwords, configure enhanced login features, and implement secure remote login with SSH. It is also very important to keep the operating system up to date. Other ways to harden a device are to force periodic password changes, enforce strong passwords, and to prevent reuse of passwords. Finally, Linux clients and servers use logfiles to record the operation of the system and important events. A number of different logfiles are maintained including application logs, event logs, service logs, and system logs. Server logs record activities that are conducted by remote users who access system services. It is important to know the location of different logs in the Linux file system so that they can be accessed and monitored for problems.

- The Linux File System

Linux supports a number of different file systems that vary by speed, flexibility, security, size, structure, logic, and more. Some of the file systems that are supported by Linux are ext2, ext3, ext4, NFS, and CDFS. File systems are mounted on partitions and accessed through mounting points, or directories. Windows drive letters are examples of mounting points. The mount command can be used to display details of the file systems that are currently mounted on a Linux computer. The root file system is represented by the “/” symbol. It contains all of the files in the computer by default. Linux uses file permissions to control who is permitted to have different types of access to files and directories. Permissions include read (r), write (w), and execute (x). Files and directories have permissions that are assigned for users, groups, and others. The permissions for files and folders are displayed with the ls -l command. This command also displays the links for a file. Hard links create another file with a different name that is linked to the same place in the file system. The owner of the file and the group for the file are also displayed along with the date and time of the last modification to the file. File permissions are powerful features of the Linux file system and can’t be violated. Only the root user can override file permissions. Because of the power of the root user, root access should be carefully controlled. Hard links are created with the ln command. Changes to one of the hard-linked files are also made to the original file. Symbolic links, or symlinks, are similar to hard links in that a change to the linked file is reflected in the original file. Symbolic links have several advantages over hard links.

- Working with Linux GUI

The X Windows, or X11, system is a basic software framework that includes functions for creating, controlling, and configuring a windows GUI in a point-and-click interface. Different vendors use the X Windows system to create different windows manager GUIs for Linux. Examples of windows managers are Gnome and KDE. The Ubuntu Linux distribution uses Gnome 3 by default. The Gnome 3 desktop consists of the Apps Menu, Ubuntu Dock, Top Bar, Calendar and System Message tray, the Activities area, and the Status Menu.

- Working on a Linux Host

In order to install applications on Linux hosts, programs called package managers are used. Packages are software applications and all of their supporting files. Package managers are extremely helpful for installing complex software applications from centralized package repositories that are accessible over the internet. Different Linux distributions use different package managers. For example, Arch Linux uses pacman, Debian uses dpkg as the base package manager and apt to communicate with dpkg. Ubuntu also uses apt. Package manager CLI commands are used to install, remove, and update software packages. Upgrade commands upgrade all currently installed packages. Package management can also be performed in a GUI. Software processes are instances of computer programs that are running. Multitasking operating systems can run many processes at the same time. Forking is a method that the kernel uses to allow a running process to copy itself. The ps command lists the running processes, top displays information about running processes dynamically, and kill is used to remove, restart, or pause running processes. While Linux is considered to be better protected against malicious software (malware) than other operating systems, it is still susceptible to Trojan horses, worms, and other types of malware. Linux is usually attacked through its services and processes. Out of date software is often vulnerable to attack. Threat actors can probe a device for open ports that are linked to out of date server processes. With this knowledge, attacks can be launched. It is important to keep the operating system and its components and applications up to date. The chkrootkit program is designed to detect rootkit malware. Rootkits are deep level malware programs that are very difficult to detect and remove. They can change the fundamental operation of the operating system itself and can be used to create unauthorized access to systems. Piping commands uses the “|” symbol to chain different commands together by using the output of one command as the input for another.

# 1.8.2 QUIZ: Linux Overview

