# Powershell Basics

- PS : stands for PowerShell

<img width="1279" height="422" alt="Screenshot (3103)" src="https://github.com/user-attachments/assets/02d0babd-e366-444a-a6c9-3091fca07e7a" />

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

# 3.0 Piping, Filtering, and Sorting Data

# 4.0 System and Network Information

# 5.0 Real-Time System Analysis

# 6.0 Scripting

# Others
