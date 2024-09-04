# The typical Booting Process
![Screenshot (369)](https://github.com/mahtokamal/OS_foundational_concepts/assets/62587491/d8bb3dcc-3b41-43f9-8399-e1ec97cb06ab)

![Screenshot (372)](https://github.com/mahtokamal/OS_foundational_concepts/assets/62587491/234fed7f-a701-42a5-9e26-a9fadd66de2e)

![Screenshot (373)](https://github.com/mahtokamal/OS_foundational_concepts/assets/62587491/6e68b5ec-a0ef-4ed7-92ac-9d0d4ea5485b)

# Understanding Windows OS Boot Process
When you press Power button ON to till you get the user login interface is known as boot process or booting of an Operating System.

**Cold booting  Vs Warm booting**
|Cold booting|warm booting|
|------------|------------|
|System Started with Power button |Restarting of running System|
|Power button |CTRL+ALT+DEL(RESTART)|
|BIOS/UEFI |Active Partition|
|MBR |BCD (Boot Configuration Data)|
|Active Partitions (Disk 0 or sector )||
|BCD (Boot Configuration Data)||

**BIOS  Vs UEFI**
|BIOS Firmware|UEFI Firmware|
|------------|------------|
|Basics Input OUtput System|Unified Extensible Firmware Inteface|
|Supports CLI(Keyboard only) |Supports GUI (Keyboard + Mouse)|
|Legacy boot |Secure boot|
|MBR(Master Boot Record) file partitioning |GUID(Globally Unique Identifiers) partitiong Table(GPT) + MBR(backward compatibility) partitioning formats|
|||
|||

**MBR  Vs GPT**<br>
When the system is powered on, it runs the BIOS program stored in the read-only memory(ROM-chips).
|MBR(Master Boot Record)|GUID Partition Table(GPT)|
|------------|------------|
|allows upto 2TB of partition|allowss more than 2TB of partition (and upto 256 TB|
|4 Primary partitions |128 primary partitions|
|Legacy boot |Secure boot|
|MBR(Master Boot Record) file partitioning |GUID(Globally Unique Identifiers) partitiong Table(GPT) + MBR(backward compatibility) partitioning formats|
|||
|||

![Screenshot (376)](https://github.com/mahtokamal/OS_foundational_concepts/assets/62587491/63795121-5415-4773-be92-3b32184229a2)

![Screenshot (377)](https://github.com/mahtokamal/OS_foundational_concepts/assets/62587491/57ebfc7c-1309-4bc3-8280-c1f8d655161c)

![Screenshot (378)](https://github.com/mahtokamal/OS_foundational_concepts/assets/62587491/8fc75f7f-881c-4241-a966-ca650458adab)

![Screenshot (379)](https://github.com/mahtokamal/OS_foundational_concepts/assets/62587491/f10cac5f-0e4a-430d-ba7f-13571df671e2)

![Screenshot (380)](https://github.com/mahtokamal/OS_foundational_concepts/assets/62587491/b30d5e4c-4ec9-4d5b-adf4-d8f6d2785c15)

**Storage structure of a Hard Disk** <br>
![Screenshot (374)](https://github.com/mahtokamal/OS_foundational_concepts/assets/62587491/1abe7cfd-0411-463e-a081-9ecbb4ddf9ad)


# Windows Boot Process in generalized way
![2020-11-11_153958](https://github.com/user-attachments/assets/f517caac-dd6e-4579-b478-79a4cb87ba7e)

**Firmware :** Firmware is software coded non-volatile memory devices such as:

1. ROM (Read only memory)
2. EPROM (Electronically Programmable Read only memory)
3. EEPROM (Electronically Erasable Programmable read only memory)
4. Flash memory

- BIOS : BIOS firmware was created in the early 1980s and works in the same way it did when it was created. As computers evolved, it became difficult
         for BIOS firmware to support all the new features requested by users.
- UEFI : UEFI was designed to replace BIOS and support the new features.

- UEFI Boots much faster than BIOS systems, especially for Windows machines.
- UEFI Firmware is usually loaded into flash memory or EEPROM, making it easier to update and patch.
- UEFI offers SECURED BOOT mode which only allows verified drivers to load.
- UEFI offers drive support of up to 9 zettabytes, while BIOS only works with 2 terabytes.

<a href="https://en.wikipedia.org/wiki/UEFI#Features">UEFI in details</a> <br>
<a href="https://www.quora.com/Are-EFI-and-UEFI-the-same-thing-What-is-the-easiest-way-to-explain-to-me-what-UEFI-BIOS-GPT-DOS-MBR-and-EFI-partitioning-is-All-the-websites-and-videos-I-watch-are-too-advanced-for-me">UEFI vs EFI vs BIOS </a><br>
<a href="https://www.geeksforgeeks.org/uefiunified-extensible-firmware-interface-and-how-is-it-different-from-bios/">BIOSvsUEFI</a><br>

<a href="https://www.freecodecamp.org/news/uefi-vs-bios/#:~:text=UEFI%20stands%20for%20Unified%20Extensible,storing%20it%20on%20the%20firmware.">BIOS-UEFI</a><br>

# Demystifying each steps of Window OS booting
![Windows_OS_booting](https://github.com/mahtokamal/OS_foundational_concepts/assets/62587491/6bc92ea3-0fb5-4a5c-b259-054d227e0de7)


# Why do we required to know about Booting proess as a Cyber Security enthusiast?
- **Rootkits** are a type of malware that hide themselves and other applications. They typically run in kernel mode, so they have the same privileges as the operating system and can sometimes start before it. Because traditionally, anti-malware software doesn’t load until after the kernel and boot drivers do, rootkits often exploit weaknesses in the startup process:

- **Firmware Rootkits** overwrite the PC’s BIOS or other hardware firmware so the rootkit can start before the OS even loads

- **Bootkits** replace the OS bootloader to load the bootkit before the OS

- **Kernel rootkits** replace a portion of the OS kernel so the rootkit can start when the OS loads

- **Driver rootkits** pretend to be a boot driver that the OS uses to communicate with PC

- **Avenues of Attack** an exposed operating system can be easily used to further Offensive goals such as pivots or compromised to steal data

**1. System Starup<br>**
BIOS :<br>
   Power ON -> BIOS/UEFI
   BIOS - Intialtize hardware and perfroms (POST program) to check hardware components (CPU, RAM, keyboard, and storage devices).
   BIOS locates the boot device (HDD, SSD, USB) by reading the boot sector.<br>
UEFI:<br>
   UEFI initializes hardware and performs POST<br>
   UEFI looks for an EFI boot partition to locate the bootloader.<br>
> [!NOTE]   
> if POST runs successfully then control goes to firmware to find boot device, if not then it generates beep code(a series of audible beeps) or message depending upon error and it halts the further booting process.

**2. Bootloader**
BIOS(MBR) finds the boot device using MBR(Master Boot Record) by reading the boot sector of OS and reads BCD(Boot configuration data) then loads windows OS bootlodaer(winload.exe/BIOS or winload.efi/UEFI).
Windows boot manager (bootmgr.exe/BIOS) present a menu to select if multiple OS or dual boot is available.
From this point the Boot Loader takes over and starts the Operating System. 
 
> [!IMPORTANT]   
> MBR is at the first sector of the HDD, whereas the VBR(volume boot record) is at first sector of a partition inside the HDD.
> The MBR has a jump instruction to go to the 1st sector in the VBR.
> VBR is platform dependent (e.g. Windows OS), while MBR is not.

UEFI<br>

UEFI boot manager(bootmgfw.efi/UEFI) does the same hardware checks as BIOS, but instead of using the MBR it reads an EFI Partition. The EFI Partition contains UEFI Boot Managers(bootmgfw.efi).
From this point onwards, the UEFI Boot Manager takes over and starts the Operating System.

The windows bootloader(winload.exe/BIOS or winload.efi/UEFI) takes over everything from here to load kernel image(NToskrnl.exe), driver
> [!NOTE]   
> Windows 2003 and older used NTLDR(bootloader) or New Technology Loader
> Windows 7 Service Pack 1 and newer OS editions or versions uses bootmgr bootloader.

**3. Windows System Initializtions (NToskrnl.exe)**
Here is the simplified version of the Windows Boot Process from the kernel (ntoskrnl.exe) to the execution of LogonUi.exe or winlogon.exe (depending upon the OS version 
architecture) (the process that prompts for user interaction).<br>
It is broken into five steps. <br>
1. Loading the Operating System Kernel
2. Initializing the Kernel
3. Starting Subsystems
4. Starting Session 0 (SYSTEM account)
5. Starting Session 1 (ADMINISTRATOR account)

**3.1 Loading the Operating System Kernel**

**On UEFI Systems**
bootmgfw.efi reads a **BCD** (Boot Configuration Data) located in the EFI system partition to load the file winload.efi

**On BIOS Systems**
bootmgr or NTLDR reads the file **\Boot\BCD** to locate **winload.exe**
- The purpose of both winload programs is to load basic drivers and start the next part of the Windows Boot Process - loading the Kernel.

**Winload.exe** loads the Windows kernel:
- Loads essential drivers required to read data from disk
- Loads the windows kernel (ntoskernel.exe) and dependencies

**Winresume.exe** reads previously saved data from hiberfil.sys (**hibernation mode**) to restore a previous Windows instance.
- On UEFI systems, winresume.exe is named **winresume.efi**, and is located at \windows\system32\boot.

**3.2 Initializing the Kernel**
The kernel, as previously discussed, is the heart of the Operating System. Without it, the system cannot function.
In Windows, the kernel is named **Ntoskrnl.exe** and is a critical system file. It does the following tasks during the boot process:

- Loads the Windows Registry
- Loads device drivers
- Starts the system pagefile located at **C:\pagefile.sys**
- Loads **hal.dll**
   - hal.dll provides abstraction between hardware interfaces and Ntoskrnl.exe


Once the kernel is done loading it spawns **System** which hosts threads that only run in kernel mode responsible things like drivers. **System** then spawns the session management processes **smss.exe** and **csrss.exe**

**4. Starting Subsystems**
**smss.exe (Session Manager Subsystem)** does the following tasks:

- Loads environmental variables like %APPDATA% and %COMPUTERNAME%
- Populates the pagefile located in C:\pagefile.sys
- Starts the kernel and user mode sub systems.
- Starts a **csrss.exe **to manage processes and threads for each User Subsystem.

**​4.1 Kernel Subsystems**
The kernel subsystem creates and manages every resource available to Windows by interacting with drivers on the system. It controls things like:
- System power state
- Process creation and threads
- Graphical rendering
- Access Control Lists via the Security Reference Monitor

**NOTE :** It is important to understand - users cannot interact directly with any kernel-mode process or even see them

**4.2 User Subsystems**
**Important:** This is the first part of Windows that a user is able to manipulate.
The user subsystem manages all user applications like process creation, internet connectivity, and object access through API calls to **hal.dll**

User Subsystems run in **Session 0** and **Session 1**

![winboot1](https://github.com/mahtokamal/OS_foundational_concepts/assets/62587491/c99ac486-7707-4cf9-9802-23a93e2dc734)

**4.2.1 User Subsystem Session 0**
Session 0 is for security and high privilege processes such as services. They are run in a separate session to isolate them from individual user’s processes.

- smss.exe installs the Win32 subsystem kernel and user mode components (win32k.sys - kernel; winsrv.dll - user; and csrss.exe - user.)
  - **csrss.exe**- The Client/Server Runtime Subsystem supports process / thread creation and management.
  - **wininit.exe** marks itself as critical, initializes the Windows temp directory, loads the rest of the registry, and starts user mode scheduling. It also installs 
   programs that require a reboot to finish the install process. **It also starts:**

   - **lsm.exe** - the Local Session Manager (LSM) handles all sessions of a system (both remote desktop sessions and local system sessions.)
   - **lsass.exe** - the Local Security Authority Subsystem (LSASS) provides user authentication services, manages the local security policy, and generates access tokens.
   - **services.exe** the Services Control Manager (SCM) loads AutoStart services, using LSASS to authenticate if they run as something other than System.

 - **wininit.exe** then waits for system shutdown to undo everything it started.

> [!IMPORTANT]
> Processes in User Subsystem Session 0 are created using the highest permissions available to a User in Windows - **SYSTEM**<br>
>**System** has more permissions than an administrative account <br>
> represents the Windows Operating System <br>
> *Can be tricked into executing malicious commands via services <br>

<a href="https://attack.mitre.org/techniques/T1569/">Mitre ATT&CK: System Services</a><br>
<a href="https://attack.mitre.org/techniques/T1574/011/">Mitre ATT&CK: Hijack Execution Flow: Services Registry</a>

**4.2.2 User Subsystem Session 1**
Session 1 is for the first interactive user (note: each session gets its own copy of csrss.exe.) Session 1 and up are standard user sessions. This includes everyone from the default **Administrator** to custom accounts created. It is the entire desktop experience on Windows.

It does the following, in order, for Session 1 and up:
1. Spawn a Session 1 ( or higher) **csrss.exe**
2. Spawn **Winlogon.exe** which by default prompts for credentials with **logonui.exe**
3. Spawn **userinit.exe** which creates an account token and creates a custom environment
4. Spawn **explorer.exe** as the customized graphical environment.

> [!IMPORTANT]
> Hundreds of Processes in **User Subsystem Session 1 and up** are started automatically as a standard user to include administrative accounts. This potentially opens up the system to vulnerabilities such as: <br>
> <a href="https://attack.mitre.org/techniques/T1547/001/">Mitre ATT&CK: Boot or Logon AutoStart Execution via Registry Keys</a><br>
> <a href="https://attack.mitre.org/techniques/T1037/001/">Mitre ATT&CK: Boot or Logon Initialization Scripts</a><br>
> <a href="https://attack.mitre.org/techniques/T1546/013/">Mitre ATT&CK: PowerShell Profile Script Execution</a><br>
> The potential damage of these vulnerabilities is limited to the permissions of the account it executed on.

5. 
6. 



# List of References
https://os.cybbh.io/public/os/latest/006_windows_boot_process/winboot_fg.html <br>
https://en.wikipedia.org/wiki/Booting_process_of_Windows <br>
https://en.m.wikipedia.org/w/index.php?title=Windows_Boot_Manager&diffonly=true#Boot_Configuration_Data <br>
