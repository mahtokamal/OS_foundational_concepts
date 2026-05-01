# Powershell Basics

- PS : stands for PowerShell

<img width="1279" height="422" alt="Screenshot (3103)" src="https://github.com/user-attachments/assets/02d0babd-e366-444a-a6c9-3091fca07e7a" />

- $PSVersionTable
<img width="1841" height="454" alt="Screenshot (3110)" src="https://github.com/user-attachments/assets/353992b3-89c0-452b-9fec-125a506a9092" />

PowerShell is a cross-platform task automation solution made up of a command-line shell, a scripting language, and a configuration management framework. PowerShell runs on Windows, Linux, and macOS.It combines a command-line interface and a scripting language built on the .NET framework. Unlike older text-based command-line tools, PowerShell is object-oriented, which means it can handle complex data types and interact with system components more effectively. Initially exclusive to Windows, PowerShell has lately expanded to support macOS and Linux, making it a versatile option for IT professionals across different operating systems.

**A Brief History of PowerShell**

PowerShell was developed to overcome the limitations of existing command-line tools and scripting environments in Windows. In the early 2000s, as Windows was increasingly used in complex enterprise environments, traditional tools like cmd.exe and batch files fell short in automating and managing these systems. Microsoft needed a tool that could handle more sophisticated administrative tasks and interact with Windows’ modern APIs.

Jeffrey Snover, a Microsoft engineer, realised that Windows and Unix handled system operations differently—Windows used structured data and APIs, while Unix treated everything as text files. This difference made porting Unix tools to Windows impractical. Snover’s solution was to develop an object-oriented approach, combining scripting simplicity with the power of the .NET framework. Released in 2006, PowerShell allowed administrators to automate tasks more effectively by manipulating objects, offering deeper integration with Windows systems.

As IT environments evolved to include various operating systems, the need for a versatile automation tool grew. In 2016, Microsoft responded by releasing PowerShell Core, an open-source and cross-platform version that runs on Windows, macOS, and Linux.

**The Power in PowerShell**

To fully grasp the power of PowerShell, we first need to understand what an object is in this context.

In programming, an object represents an item with properties (characteristics) and methods (actions). For example, a car object might have properties like Color, Model, and FuelLevel, and methods like Drive(), HonkHorn(), and Refuel().

Similarly, in PowerShell, objects are fundamental units that encapsulate data and functionality, making it easier to manage and manipulate information. An object in PowerShell can contain file names, usernames or sizes as data (properties), and carry functions (methods) such as copying a file or stopping a process.

The traditional Command Shell’s basic commands are text-based, meaning they process and output data as plain text. Instead, when a cmdlet (pronounced command-let) is run in PowerShell, it returns objects that retain their properties and methods. This allows for more powerful and flexible data manipulation since these objects do not require additional parsing of text.

# 1.0 PowerShell Basics

**1.1 Basic Syntax: Verb-Noun**

PowerShell commands are known as cmdlets (pronounced command-lets). They are much more powerful than the traditional Windows commands and allow for more advanced data manipulation.
Cmdlets follow a consistent Verb-Noun naming convention. This structure makes it easy to understand what each cmdlet does. The Verb describes the action, and the Noun specifies the object on which action is performed. For example:

- Get-Content: Retrieves (gets) the content of a file and displays it in the console.
- Set-Location: Changes (sets) the current working directory.


**1.2 Basic cmdlets**

- Get-Command: It list all available cmdlets, functions, aliases, and scripts that can be executed in the current PowerShell session. It’s an essential tool for discovering what commands one can use.

<img width="1766" height="721" alt="Screenshot (3104)" src="https://github.com/user-attachments/assets/a550f658-1d5e-4624-82a3-7abeb6d0c6eb" />

For each **CommandInfo** object retrieved by the cmdlet, some essential information (properties) is displayed on the console. It’s possible to filter the list of commands based on displayed property values. For example, if we want to display only the available commands of type “function”, we can use **-CommandType "Function"**, as shown below:

<img width="1767" height="428" alt="Screenshot (3105)" src="https://github.com/user-attachments/assets/4ad41830-bf23-4a58-bac5-92d7f09deecd" />

- Get-Help: it provides detailed information about cmdlets, including usage, parameters, and examples. It’s the go-to cmdlet for learning how to use PowerShell commands.Synatx : Get-Help <cmdlet-name> --> Get-Help Get-Date
  - get-help Get-Date -examples -> To see the examples
  - get-help Get-Date -detailed -> For more information
  - get-help Get-Date -full ->  For technical information
  - get-help Get-Date -online -> For online help
<img width="1476" height="1032" alt="Screenshot (3106)" src="https://github.com/user-attachments/assets/13ae748c-d603-4130-8c18-d548e7c80357" />

To make the transition easier for IT professionals, PowerShell includes aliases —which are shortcuts or alternative names for cmdlets— for many traditional Windows commands. Indispensable for users already familiar with other command-line tools, **Get-Alias** lists all aliases available. For example, **dir** is an alias for **Get-ChildItem**, and cd is an alias for **Set-Location**.

<img width="1758" height="640" alt="Screenshot (3107)" src="https://github.com/user-attachments/assets/6b5ed0e1-7ec1-47ea-bc5c-84de76b7dfb7" />

**1.3 Where to Find and Download Cmdlets**

Another powerful feature of PowerShell is the possibility of extending its functionality by downloading additional cmdlets from online repositories.

NOTE: Please note that the cmdlets listed in this section require a working internet connection to query online repositories. The attached machine doesn't have access to the internet, therefore these commands won't work in this environment.

To search for modules (collections of cmdlets) in online repositories like the PowerShell Gallery, we can use **Find-Module**. Sometimes, if we don’t know the exact name of the module, it can be useful to search for modules with a similar name. We can achieve this by filtering the **Name** property and appending a wildcard **(*)** to the module’s partial name, using the following standard PowerShell syntax: **Cmdlet -Property "pattern*"**.

<img width="1770" height="464" alt="Screenshot (3108)" src="https://github.com/user-attachments/assets/bbb1a6b5-a936-4668-8db4-47b614ca5752" />

Once identified, the modules can be downloaded and installed from the repository with **Install-Module**, making new cmdlets contained in the module available for use.

<img width="1769" height="286" alt="Screenshot (3109)" src="https://github.com/user-attachments/assets/637926c1-01af-4d18-a3b3-ac1d10fa246d" />

# 2.0 Navigating the File System and Working with Files
- Get-ChildItem : (dir,ls)
- Set-Location : (cd)
- New-Item
- Remove-Item : (rmdir, del)
- Copy-Item : (copy,)
- Move-Item : (move)
- Get-Content : (type, cat)

PowerShell provides a range of cmdlets for navigating the file system and managing files, many of which have counterparts in the traditional Windows CLI.

Similar to the dir command in Command Prompt (or ls in Unix-like systems), Get-ChildItem lists the files and directories in a location specified with the -Path parameter. It can be used to explore directories and view their contents. If no Path is specified, the cmdlet will display the content of the current working directory. <br>

<img width="1771" height="647" alt="Screenshot (3111)" src="https://github.com/user-attachments/assets/494b9b3b-b70a-4b5f-a86f-c5f533eda5d9" />


To navigate to a different directory, we can use the Set-Location cmdlet. It changes the current directory, bringing us to the specified path, akin to the cd command in Command Prompt.

<img width="1685" height="164" alt="Screenshot (3112)" src="https://github.com/user-attachments/assets/f920ebb9-219d-460a-93d5-f687c658815a" />

While the traditional Windows CLI uses separate commands to create and manage different items like directories and files, PowerShell simplifies this process by providing a single set of cmdlets to handle the creation and management of both files and directories.

To create an item in PowerShell, we can use New-Item. We will need to specify the path of the item and its type (whether it is a file or a directory).

<img width="1762" height="646" alt="Screenshot (3113)" src="https://github.com/user-attachments/assets/8b9e8e22-3862-4488-9879-58269ca497b7" />

Similarly, the Remove-Item cmdlet removes both directories and files, whereas in Windows CLI we have separate commands rmdir and del.

<img width="1769" height="166" alt="Screenshot (3114)" src="https://github.com/user-attachments/assets/f988cde7-b219-4984-b630-2f0661550687" />

We can copy or move files and directories alike, using respectively Copy-Item (equivalent to copy) and Move-Item (equivalent to move).

<img width="1758" height="528" alt="Screenshot (3115)" src="https://github.com/user-attachments/assets/a78a67a7-51c7-4222-b3d2-2452b8946457" />

Finally, to read and display the contents of a file, we can use the Get-Content cmdlet, which works similarly to the type command in Command Prompt (or cat in Unix-like systems).

<img width="1763" height="418" alt="Screenshot (3116)" src="https://github.com/user-attachments/assets/02884950-3b65-420a-b6ed-90a786c434f0" />

# 3.0 Piping, Filtering, and Sorting Data

Piping is a technique used in command-line environments that allows the output of one command to be used as the input for another. This creates a sequence of operations where the data flows from one command to the next. Represented by the | symbol, piping is widely used in the Windows CLI, as introduced earlier in this module, as well as in Unix-based shells.

In PowerShell, piping is even more powerful because it passes objects rather than just text. These objects carry not only the data but also the properties and methods that describe and interact with the data.

For example, if you want to get a list of files in a directory and then sort them by size, you could use the following command in PowerShell:

<img width="1773" height="495" alt="Screenshot (3118)" src="https://github.com/user-attachments/assets/c20466da-e7fb-48b9-8024-9104679a8eca" />

Here, Get-ChildItem retrieves the files (as objects), and the pipe (|) sends those file objects to Sort-Object, which then sorts them by their Length (size) property. This object-based approach allows for more detailed and flexible command sequences.

In the example above, we have leveraged the Sort-Object cmdlet to sort objects based on specified properties. Beyond sorting, PowerShell provides a set of cmdlets that, when combined with piping, allow for advanced data manipulation and analysis.

To filter objects based on specified conditions, returning only those that meet the criteria, we can use the Where-Object cmdlet. For instance, to list only .txt files in a directory, we can use:

<img width="1756" height="447" alt="Screenshot (3119)" src="https://github.com/user-attachments/assets/19c576bf-d522-4be1-b4b2-84ea1fd97d99" />

Here, Where-Object filters the files by their Extension property, ensuring that only files with extension equal (-eq) to .txt are listed.

The operator -eq (i.e. "equal to") is part of a set of comparison operators that are shared with other scripting languages (e.g. Bash, Python). To show the potentiality of the PowerShell's filtering, we have selected some of the most useful operators from that list:

-ne: "not equal". This operator can be used to exclude objects from the results based on specified criteria.
-gt: "greater than". This operator will filter only objects which exceed a specified value. It is important to note that this is a strict comparison, meaning that objects that are equal to the specified value will be excluded from the results.
-ge: "greater than or equal to". This is the non-strict version of the previous operator. A combination of -gt and -eq.
-lt: "less than". Like its counterpart, "greater than", this is a strict operator. It will include only objects which are strictly below a certain value.
-le: "less than or equal to". Just like its counterpart -ge, this is the non-strict version of the previous operator. A combination of -lt and -eq.
Below, another example shows that objects can also be filtered by selecting properties that match (-like) a specified pattern:

<img width="1759" height="352" alt="Screenshot (3120)" src="https://github.com/user-attachments/assets/060998eb-62da-4159-92cd-f8b766e6ed2e" />

The next filtering cmdlet, Select-Object, is used to select specific properties from objects or limit the number of objects returned. It’s useful for refining the output to show only the details one needs.

<img width="1765" height="426" alt="Screenshot (3121)" src="https://github.com/user-attachments/assets/9862fd7f-94c1-4e2b-b4df-3f429f9571b6" />

The cmdlets pipeline can be extended by adding more commands, as the feature isn’t limited to just piping between two cmdlets. As an exercise, try and build a pipeline of cmdlets to sort and filter the output with the goal of displaying the largest file in the C:\Users\captain\Documents\captain-cabin directory.

Click here to look at a possible solution. Don’t cheat!

<img width="1788" height="429" alt="Screenshot (3117)" src="https://github.com/user-attachments/assets/765510d0-ea89-4c2f-9019-80ef08c822f3" />


The last in this set of filtering cmdlets is Select-String. This cmdlet searches for text patterns within files, similar to grep in Unix-based systems or findstr in Windows Command Prompt. It’s commonly used for finding specific content within log files or documents.

<img width="1770" height="207" alt="Screenshot (3122)" src="https://github.com/user-attachments/assets/190cf516-2495-4fca-ae5e-9f3bdb1e434c" />

The Select-String cmdlet fully supports the use of regular expressions (regex(opens in new tab)). This advanced feature allows for complex pattern matching within files, making it a powerful tool for searching and analysing text data.

# 4.0 System and Network Information

PowerShell was created to address a growing need for a powerful automation and management tool to help system administrators and IT professionals. As such, it offers a range of cmdlets that allow the retrieval of detailed information about system configuration and network settings.

The Get-ComputerInfo cmdlet retrieves comprehensive system information, including operating system information, hardware specifications, BIOS details, and more. It provides a snapshot of the entire system configuration in a single command. Its traditional counterpart systeminfo retrieves only a small set of the same details.

<img width="1771" height="457" alt="Screenshot (3123)" src="https://github.com/user-attachments/assets/f38c3ee4-d76d-4049-be77-8a6a0373d057" />

Essential for managing user accounts and understanding the machine’s security configuration, Get-LocalUser lists all the local user accounts on the system. The default output displays, for each user, username, account status, and description.

<img width="1764" height="420" alt="Screenshot (3124)" src="https://github.com/user-attachments/assets/d1b20594-ad9d-46f8-b612-895fbf73bcc3" />

Similar to the traditional ipconfig command, the following two cmdlets can be used to retrieve detailed information about the system’s network configuration.

<img width="1764" height="455" alt="Screenshot (3125)" src="https://github.com/user-attachments/assets/f7d4c409-9f4e-43d7-802a-5329aff5ab44" />

Get-NetIPConfiguration provides detailed information about the network interfaces on the system, including IP addresses, DNS servers, and gateway configurations.

In case we need specific details about the IP addresses assigned to the network interfaces, the Get-NetIPAddress cmdlet will show details for all IP addresses configured on the system, including those that are not currently active.

<img width="1469" height="1013" alt="Screenshot (3126)" src="https://github.com/user-attachments/assets/a2903fa3-a731-4f0f-ac01-53df1427727d" />

These cmdlets give IT professionals the ability to quickly access crucial system and network information directly from the command line, making it easier to monitor and manage both local and remote machines.

# 5.0 Real-Time System Analysis

To gather more advanced system information, especially concerning dynamic aspects like running processes, services, and active network connections, we can leverage a set of cmdlets that go beyond static machine details.

Get-Process provides a detailed view of all currently running processes, including CPU and memory usage, making it a powerful tool for monitoring and troubleshooting.

<img width="1769" height="454" alt="Screenshot (3127)" src="https://github.com/user-attachments/assets/afb21bc4-33a9-49d6-914a-c09c15a20b4f" />

Similarly, Get-Service allows the retrieval of information about the status of services on the machine, such as which services are running, stopped, or paused. It is used extensively in troubleshooting by system administrators, but also by forensics analysts hunting for anomalous services installed on the system.

<img width="1762" height="493" alt="Screenshot (3128)" src="https://github.com/user-attachments/assets/222bb954-415b-4e1a-b8e9-0ef31970f131" />

To monitor active network connections, Get-NetTCPConnection displays current TCP connections, giving insights into both local and remote endpoints. This cmdlet is particularly handy during an incident response or malware analysis task, as it can uncover hidden backdoors or established connections towards an attacker-controlled server.

<img width="1760" height="707" alt="Screenshot (3129)" src="https://github.com/user-attachments/assets/74a557db-18c2-4ed4-8a7f-aa4b33602f1f" />

Additionally, we are going to mention Get-FileHash as a useful cmdlet for generating file hashes, which is particularly valuable in incident response, threat hunting, and malware analysis, as it helps verify file integrity and detect potential tampering.

<img width="1762" height="281" alt="Screenshot (3130)" src="https://github.com/user-attachments/assets/6dcc84b2-2ce7-4c13-bb32-436387988eb1" />

You can also view the Alternate Data Streams (ADS) attached to a file through PowerShell as shown below: (If you are not sure what ADS is, we have covered it in detail in the Windows Fundamentals 1 room)

<img width="1765" height="854" alt="Screenshot (3131)" src="https://github.com/user-attachments/assets/ba89fbe2-574d-4545-8588-bab9f483b002" />

In the output above, you can see two streams that are attached to the file C:\House\house_log.txt:

:$DATA is the default data stream of every NTFS file. It contains the normal file contents and is not an ADS.

housinginginfo is the Alternate Data Stream (ADS) added to this file. It appears as house_log.txt:housinginfo, which means an extra hidden stream named housinginfo is attached to this file.

Note: The ADS example shown above is from a file of a different machine and will not be available to you in the attached VM.

These cmdlets collectively provide a comprehensive set of tools for real-time system monitoring and analysis, proving especially useful to incident responders and threat hunters.
# 6.0 Scripting
Scripting is the process of writing and executing a series of commands contained in a text file, known as a script, to automate tasks that one would generally perform manually in a shell, like PowerShell.

Simply speaking, scripting is like giving a computer a to-do list, where each line in the script is a task that the computer will carry out automatically. This saves time, reduces the chance of errors, and allows to perform tasks that are too complex or tedious to do manually. As you learn more about shells and scripting, you’ll discover that scripts can be powerful tools for managing systems, processing data, and much more.

Learning scripting with PowerShell goes beyond the scope of this room. Nonetheless, we must understand that its power makes it a crucial skill across all cyber security roles.

For blue team professionals such as incident responders, malware analysts, and threat hunters, PowerShell scripts can automate many different tasks, including log analysis, detecting anomalies, and extracting indicators of compromise (IOCs). These scripts can also be used to reverse-engineer malicious code (malware) or automate the scanning of systems for signs of intrusion.

For the red team, including penetration testers and ethical hackers, PowerShell scripts can automate tasks like system enumeration, executing remote commands, and crafting obfuscated scripts to bypass defences. Its deep integration with all types of systems makes it a powerful tool for simulating attacks and testing systems’ resilience against real-world threats.

Staying in the context of cyber security, system administrators benefit from PowerShell scripting for automating integrity checks, managing system configurations, and securing networks, especially in remote or large-scale environments. PowerShell scripts can be designed to enforce security policies, monitor systems health, and respond automatically to security incidents, thus enhancing the overall security posture.

Whether used defensively or offensively, PowerShell scripting is an essential capability in the cyber security toolkit.

Before concluding this task about scripting, we can’t go without mentioning the Invoke-Command cmdlet.

Invoke-Command is essential for executing commands on remote systems, making it fundamental for system administrators, security engineers and penetration testers. Invoke-Command enables efficient remote management and—combining it with scripting—automation of tasks across multiple machines. It can also be used to execute payloads or commands on target systems during an engagement by penetration testers—or attackers alike.

Let us discover some example usage for this powerful cmdlet by consulting the Get-Help "examples" page:

<img width="1765" height="886" alt="Screenshot (3132)" src="https://github.com/user-attachments/assets/5c1e93b0-f1e9-4b79-9a36-28eebc000640" />

The first two examples provided by the Get-Help "examples" page and reported above are enough to grasp the simplicity and power of the Invoke-Command cmdlet.

The first example shows how the cmdlet can be very easily combined with any custom script to automate tasks on remote computers.

The second example demonstrates that we don't need to know how to script to benefit from the power of Invoke-Command. In fact, by appending the -ScriptBlock { ... } parameter to the cmdlet's syntax, we can execute any command (or sequence of commands) on the remote computer. The result would be the same as if we were typing the commands in a local PowerShell session on the remote computer itself.

# Practical
- Get-Command -> shows lists of all cmdlet, scripts, function and aliases.
   - Get-Command -CommandType "Function/Cmdlet/Alias" -> list all command based on either Function, Cmdlet or Alias
- Get-Help: -> info about specific command. Example : Get-Help Get-Date -Examples
- Get-Alias -> 
- Get-ChildItem(dir,ls) -> shows list of all available files and directories within a directory.
- Set-Location(cd) -> Change the location of directory
   - Set-Location -Path "location" -> Set-Location -Path ".\Documents"
- Get-Location (pwd) ->
   - Get-Location
- New-Item -> creates a new directory or file on a specified path
   - For directory -> New-Item -Path ".\PowerShell_Directory" ItemType "Directory"
   - For file -> New-Item -Path ".\PowerShell_Directory\test.txt" ItemType "File"
- Remove-Item : (rmdir, del, erase) -> deletes a file and directory from a given path.
   - Remove-Item -Path ".\newpowershell\powershell.txt"
   - Remove-Item -Path ".\newpowershell\"
- Copy-Item : (copy,) -> copies files and directories from source path to destination path.
   - Example -> Copy-Item -Path ".\Powershell\testtext.txt" -Destination ".\PracticePowershell\"
   - 
- Move-Item : (move) -> moves files and directories from source path to destination path.
   - Example -> Move-Item -Path ".\Powershell\testtext.txt" -Destination ".\PracticePowershell\"
- Rename-Item :
   - Example -> Rename-Item ".\powershell_test\" powershell_test2
- Get-Content : (type, cat) -> to view contents of a file.
   - Example : Get-Content ".\powershell\testtext.txt"
- Set-Content
   - Example : Set-Content ".\testfile.txt" "welcome to the PowerShell MasteClass!"
- Add-content : It appends to the file
   - Example -> Add-Content .\testfile.txt "Welcome again!"
- Clear-Content :
   - Example -> Clear-Content .\testfile.txt
- Write-Output : (echo) -> prints on the terminal
   - Example : Write-Output "Hello! Welcome to the Powershell Scripting"
- Test-Path : It checks folder existence
   - Example -> Test-Path ".\powershell_test" -> if found returns true, otherwise False
- Get-History : (h, history)
- Get-Item:
- Get-ComputerInfo : It retrieves System Information
   - Example : Get-ComputerInfo
- 

# Basics command

# Powershell Advanced Cmdlets

**Get-Unique Cmdlet** <br>

Get-Unique cmdlet can be used to get the unique objects from a sorted list of objects.

**Group-Object Cmdlet** <br>
 
**Measure-Object Cmdlet** <br>

**Compare-Object Cmdlet** <br>

**Format-List Cmdlet** <br>

**Format-Wide Cmdlet** <br>

**Where-Object Cmdlet** <br>

**Get-ChildItem Cmdlet** <br>

**ForEach-Object Cmdlet** <br>

**Start-Sleep Cmdlet** <br>

**Read-Host Cmdlet** <br>

**Select-Object Cmdlet** <br>

**Sort-Object Cmdlet** <br>

**Write-Warning Cmdlet** <br>

**Write-Host Cmdlet** <br>

**Invoke-Item Cmdlet** <br>

**Invoke-Expression Cmdlet** <br>

**Measure-Command Cmdlet** <br>

**Invoke-History Cmdlet** <br>

**Add-History Cmdlet** <br>
**Get-History Cmdlet** <br>
**Get-Culture Cmdlet** <br>

# Basics 
**Date and Times**

- Get-Date
- Set-Date

# Powershell Scripting


# Others


