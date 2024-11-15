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
# 1.4 Basic Server Administration
# 1.5 The Linux File System
# 1.6 Working with GUI
# 1.7 Working on a Linux Host

