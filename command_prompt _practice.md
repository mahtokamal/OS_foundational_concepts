# 1. Command Prompt Tutorials

## 2. File and Directory

### 2.1 dir
    Description - Displays a list of files and subdirectories in a directory.
    
    Syntax - DIR [drive:][path][filename] [/A[[:]attributes]] [/B] [/C] [/D] [/L] [/N]
             [/O[[:]sortorder]] [/P] [/Q] [/R] [/S] [/T[[:]timefield]] [/W] [/X] [/4]

             [drive:][path][filename]
              Specifies drive, directory, and/or files to list.
    
    Example - help dir  or dir /? (shows all the options or switches available for dir command).
    Example - dir

    Example - dir /a (shows all files, subdirectories including hidden one in a directory.)

![Screenshot (434)](https://github.com/user-attachments/assets/58e4b009-0268-4911-b8eb-c10d7ec37b46)

![Screenshot (435)](https://github.com/user-attachments/assets/5fc85d5d-cdb5-483c-ba3d-039746f545fb)

![Screenshot (432)](https://github.com/user-attachments/assets/812b0f47-2a65-4b46-b52d-c2ebc67c05bf)

![Screenshot (433)](https://github.com/user-attachments/assets/84cf9277-3a0e-4a6e-80f7-cfaa9dd58d00)

![Screenshot (436)](https://github.com/user-attachments/assets/5535a451-4966-4ecf-8cd1-df0fbd7dcd73)

### 2.2 cd or chdir
    Description - Displays the name of or changes the current directory.
    Syntax - CHDIR [/D] [drive:][path]
             CHDIR [..]
             CD [/D] [drive:][path]
             CD [..]

    [..   Specifies that you want to change to the parent directory.]
    
    Example - 
    Output -
![Screenshot (457)](https://github.com/user-attachments/assets/0e52909c-b089-47ff-828b-53490c2ac88e)

![Screenshot (458)](https://github.com/user-attachments/assets/7ba6fe7a-4f74-4b0d-8052-7c3977eed35c)

![Screenshot (459)](https://github.com/user-attachments/assets/aa931f33-5681-4dc3-ada8-a1b180cdaa87)

### 2.3 copy, xcopy, robocopy
    Description - Copies one or more files to another location.

    Copy Syntax - COPY [/D] [/V] [/N] [/Y | /-Y] [/Z] [/L] [/A | /B ] source [/A | /B]
                  [+ source [/A | /B] [+ ...]] [destination [/A | /B]] 
    
    Xcopy - Copies files and directory trees.
    Syntax - XCOPY source [destination] [/A | /M] [/D[:date]] [/P] [/S [/E]] [/V] [/W]
                           [/C] [/I] [/-I] [/Q] [/F] [/L] [/G] [/H] [/R] [/T]
                           [/U] [/K] [/N] [/O] [/X] [/Y] [/-Y] [/Z] [/B] [/J]
                           [/EXCLUDE:file1[+file2][+file3]...] [/COMPRESS]
    
    /S  - Copies directories and subdirectories, but not empty ones.
    /E -  Copies all subdirectories, including empty ones.


    Robocopy -  Robust File Copy for Windows. XCOPY is deprecated in favor of ROBOCOPY, which offers even more advanced options for copying files and directories.
    
    Syntax - robocopy <Source> <Destination> [<File>[ ...]] [<Options>] 

             source :: Source Directory (drive:\path or \\server\share\path).
        destination :: Destination Dir  (drive:\path or \\server\share\path).
               file :: File(s) to copy  (names/wildcards: default is "*.*").

![Screenshot (465)](https://github.com/user-attachments/assets/422bb63c-c23e-466a-8265-9d24455a54cf)

![Screenshot (466)](https://github.com/user-attachments/assets/9831ba94-868d-4446-9ee2-d0b43341ab3f)

    Xcopy(Extended copy) Example
![Screenshot (467)](https://github.com/user-attachments/assets/7a6be176-fe1b-4f76-96d3-986d7dd37096)

![Screenshot (468)](https://github.com/user-attachments/assets/3f3f4335-343d-46ae-a1dd-96c80687964a)

![Screenshot (469)](https://github.com/user-attachments/assets/a1604bd6-89c1-4708-9442-61ff7c04b130)

![Screenshot (470)](https://github.com/user-attachments/assets/a04f8556-f08c-4342-919c-a609e78264ff)

![Screenshot (471)](https://github.com/user-attachments/assets/ec8e2cb3-b8e4-46ad-846a-8cf2947ccd01)

![Screenshot (472)](https://github.com/user-attachments/assets/05bf35ec-6171-40a7-9187-a772774e9278)

![Screenshot (473)](https://github.com/user-attachments/assets/5af7c08e-5639-4d41-aa86-0b535fee26e7)


![Screenshot (474)](https://github.com/user-attachments/assets/2892d2fb-5d21-4776-9b5e-05e65be2ab83)

    Robocopy(Robust File copy) Example

![Screenshot (476)](https://github.com/user-attachments/assets/26e4a13d-8f12-4ff5-bb81-e886cd778e5b)

![Screenshot (477)](https://github.com/user-attachments/assets/d9fa86fb-e2ee-422b-9163-311823b87695)

![Screenshot (479)](https://github.com/user-attachments/assets/ff11a71b-4616-4f93-9709-cb87407f1254)

![Screenshot (480)](https://github.com/user-attachments/assets/ed2755e9-2866-42cf-9c72-7300e6e7db90)




### 2.4 move
    Description - Moves files and renames files and directories.

    Syntax - 
    To move one or more files:
    MOVE [/Y | /-Y] [drive:][path]filename1[,...] destination

    To rename a directory:
    MOVE [/Y | /-Y] [drive:][path]dirname1 dirname2
    
    Example -
    Output - 

![Screenshot (481)](https://github.com/user-attachments/assets/58017199-d1d5-4e73-b616-72c3c644619d)

![Screenshot (483)](https://github.com/user-attachments/assets/d0d8c9a9-398d-4bee-8642-e72f8121ace7)
![Screenshot (484)](https://github.com/user-attachments/assets/b0308d01-937b-4cf1-a9e8-52ad1ae46a0c)
![Screenshot (485)](https://github.com/user-attachments/assets/2bafbe28-7b3f-4709-bf4d-dbda1e527a2a)

![Screenshot (486)](https://github.com/user-attachments/assets/6f517a83-827b-4620-8a63-b144a01b8f88)
![Screenshot (487)](https://github.com/user-attachments/assets/31bed46c-1592-4086-9399-060fdee3d693)

![Screenshot (488)](https://github.com/user-attachments/assets/8d59fb85-6d47-4167-b516-cd7bebd5757d)
![Screenshot (490)](https://github.com/user-attachments/assets/ae209d93-0b84-4e3d-892b-d2dcc52e3d92)


![Screenshot (491)](https://github.com/user-attachments/assets/b3cf2de0-3b5b-4534-bfdc-4898ef1a3dd4)
![Screenshot (492)](https://github.com/user-attachments/assets/64977979-00c5-464b-927a-71e645d57e4a)

### 2.5 del or erase
    Description - Deletes one or more files.

    Syntax - DEL [/P] [/F] [/S] [/Q] [/A[[:]attributes]] names
             ERASE [/P] [/F] [/S] [/Q] [/A[[:]attributes]] names
    
    Example -
    Output -

![Screenshot (475)](https://github.com/user-attachments/assets/c9db60a0-0f81-4717-b331-183bf7f47bcf)

![Screenshot (493)](https://github.com/user-attachments/assets/9cce3319-f73f-49b7-acfd-0190988ee316)
![Screenshot (494)](https://github.com/user-attachments/assets/57e6008b-702c-41af-be77-b0e90d8ed454)

    
### 2.6 mkdir or md
    Description - Creates a directory.

    Syntax - MKDIR [drive:]path
             MD [drive:]path
    
    Example -
    Output - 

![Screenshot (495)](https://github.com/user-attachments/assets/f0cd220b-4415-48a5-a709-0e03dcc3d521)
![Screenshot (496)](https://github.com/user-attachments/assets/6aebc57a-9528-48b6-b0c6-fa0a6401dddd)

### 2.7 rmdir    
    Description - Removes (deletes) a directory.

    
    /S      Removes all directories and files in the specified directory
            in addition to the directory itself.  Used to remove a directory
            tree.

    /Q      Quiet mode, do not ask if ok to remove a directory tree with /S
    
    Syntax - RMDIR [/S] [/Q] [drive:]path
             RD [/S] [/Q] [drive:]path
    
    Example -
    Output - 
![Screenshot (497)](https://github.com/user-attachments/assets/8d963db1-b1fc-4842-b106-ba4b1bdb3070)

![Screenshot (498)](https://github.com/user-attachments/assets/75cc8536-ffe0-48ba-af96-31f394d77514)

### 2.8 ren or rename
    Description - Renames a file or files.

    Syntax - RENAME [drive:][path]filename1 filename2.
             REN [drive:][path]filename1 filename2.
    
    Example -
    Output - 

![Screenshot (499)](https://github.com/user-attachments/assets/838dca30-233c-4c05-8676-c07425185a5e)
![Screenshot (500)](https://github.com/user-attachments/assets/552625c0-4d22-47b7-b39c-991059424415)


### 2.9 type
    Description - Displays the contents of a text file or files.
    Syntax - TYPE [drive:][path]filename
   
    Example - type nul > hello.txt (to create empty file )
    Example - type hello.txt (to view contents of hello.txt file)
   

![Screenshot (503)](https://github.com/user-attachments/assets/65bca345-5949-4b78-a879-6aa805dff337)
![Screenshot (504)](https://github.com/user-attachments/assets/0043642f-6809-4ff4-9ac3-966c330f55e9)
![Screenshot (505)](https://github.com/user-attachments/assets/3fdfddea-0bfc-4a39-b3ed-65bd447c7adb)
![Screenshot (506)](https://github.com/user-attachments/assets/59ac3fc7-4e7c-4394-81a6-195a9f455252)

### 2.9 echo
    Description - Displays messages, or turns command-echoing on or off.

    Syntax -  ECHO [ON | OFF]
              ECHO [message]
    Example - echo Hello! How are You??
    Example - echo Hi! > hello.txt (> is used to overwrite the value)
    Example - echo Hello!! >> hello.txt (>> is used to append it to the end of the file)
    Example - echo Bye! Bye! > hello.txt (> overwrite all existing values with Bye! Bye!)

![Screenshot (501)](https://github.com/user-attachments/assets/209cf7d4-7b96-4b0c-836e-b114abce41a7)
![Screenshot (507)](https://github.com/user-attachments/assets/e34ba4b1-2957-4209-aa9d-33be8a94cd42)

## 3. Networking
### 3.1 ping
    Description - Verifies IP-level connectivity to another TCP/IP computer by sending Internet Control Message Protocol 
    (ICMP) echo Request messages. The receipt of the corresponding echo Reply messages is displayed, along with round-trip 
    times. ping is the primary TCP/IP command used to troubleshoot connectivity, reachability, and name resolution.

    You can also use this command to test both the computer name and the IP address of the computer. If pinging the IP 
    address is successful, but pinging the computer name isn't, you might have a name resolution problem. In this case, 
    make sure the computer name you're specifying can be resolved through the local Hosts file, by using Domain Name System 
    (DNS) queries, or through NetBIOS name resolution techniques.
    
    Common starting TTL values for different operating systems:
    Windows: 128
    Linux/Unix: 64
    Cisco: 255
    Solaris/AIX: 254
    
    Syntax - 
    Example -
![Screenshot (552)](https://github.com/user-attachments/assets/11e5d722-fc8f-4f56-85a0-a04e7201e572)

    Hops - when a data packet travels from source to destination through a series of devices(network devices [Router])
    and each router is considered as a hops.Typically, a hop count starts with 0 or 1.
![Hop-count-trans](https://github.com/user-attachments/assets/5ea17a67-7d9c-4166-8864-9c1887273eec)
    The hop count between the computers in this case is 2.

### 3.2 ipconfig
    Description - Displays all current TCP/IP network configuration values and refreshes Dynamic Host Configuration 
    Protocol (DHCP) and Domain Name System (DNS) settings. Used without parameters, ipconfig displays Internet Protocol 
    version 4 (IPv4) and IPv6 addresses, subnet mask, and default gateway for all adapters.

    Syntax -  ipconfig [/allcompartments] [/? | /all |
                                 /renew [adapter] | /release [adapter] |
                                 /renew6 [adapter] | /release6 [adapter] |
                                 /flushdns | /displaydns | /registerdns |
                                 /showclassid adapter |
                                 /setclassid adapter [classid] |
                                 /showclassid6 adapter |
                                 /setclassid6 adapter [classid] ]
    Example -

![Screenshot (553)](https://github.com/user-attachments/assets/f7121f18-e381-453d-b45f-e9090c421c98)
![Screenshot (554)](https://github.com/user-attachments/assets/6e946d13-8362-4393-9f56-d512bd00dc16)

    Ipconfig/all - Displays the full TCP/IP configuration for all adapters. Adapters can represent physical interfaces, such as installed network adapters, or 
    logical interfaces, such as dial-up connections.

![Screenshot (555)](https://github.com/user-attachments/assets/62916a7e-68bc-4360-a121-dd6b4321b4b9)
![Screenshot (557)](https://github.com/user-attachments/assets/77c6314e-393e-4a5c-a844-a2aab8332208)

- Physical Address: This is the MAC address of your network adapter.
- DHCP Enabled: Indicates if the network connection is using DHCP or Static IP Address
- IPv4 Address: The IP Address of your computer
- Default Gateway: The router to which your computer is connected
- DHCP Server: Router/server that hands out IP Addresses in your network
- DNS Servers: Servers used to translate domain names to IP Addresses
- Link-Local IPv6 Address: IPv6 address of your computer (often not used)
- Lease Obtained: Date-time when your computer received the IP Address    

### 3.3 nslookup
    Description - Queries the DNS to obtain the domain name or IP address mapping. This command is use to transform the 
    given searched words into their corresponding IP addresses. Such as if i search for geeks for geeks  website then our 
    browser don’t search for geeks for geeks. It search’s the corresponding IP address associated to the geeksforgeeks 
    site. 

    Syntax - nslookup [-opt ...]             # interactive mode using default server
             nslookup [-opt ...] - server    # interactive mode using 'server'
             nslookup [-opt ...] host        # just look up 'host' using default server
             nslookup [-opt ...] host server # just look up 'host' using 'server'
    Example - nslookup www.geeksforgeeks.com
![Screenshot (558)](https://github.com/user-attachments/assets/7cd9dc9c-7d94-4d75-8a0b-cb0dbc6edaaa)

### 3.4 tracert
    Description - Traces the route that packets take to reach a destination, showing each hop(router) along the way.

    Syntax -  tracert [-d] [-h maximum_hops] [-j host-list] [-w timeout]
               [-R] [-S srcaddr] [-4] [-6] target_name
    Example -
![Screenshot (559)](https://github.com/user-attachments/assets/0845fac2-3725-4f9a-ab7a-7f2b8fb5ae70)

### 3.5 netstat
    Description - Displays protocol statistics and current TCP/IP network connections. Such as network connections, Ports, 
    routing tables, interface statistics, masquerade connections, and multicast memberships. 

    It tells us active connections with our computer and it tells us local address ,foreign address and the state of the 
    device. In local address first 8 digits specify the local address of our computer and and last 5 digits tells the port 
    number to which our computer is connected .
    
    Syntax - NETSTAT [-a] [-b] [-e] [-f] [-i] [-n] [-o] [-p proto] [-r] [-s] [-t] [-x] [-y] [interval]
    Example - netstat
    Example - netstat -an [Shows all active network connections and listening ports, with their status.]
![Screenshot (560)](https://github.com/user-attachments/assets/bce78a61-468b-4c6c-84d4-0da7d71a76ce)
![Screenshot (561)](https://github.com/user-attachments/assets/2dc0ae15-d696-4e81-9f1e-a1075d540735)

### 3.6 hostname
    Description - Displays the host name portion of the full computer name of the computer.

    Syntax - hostname
    Example - hostname
![Screenshot (562)](https://github.com/user-attachments/assets/a73e14f9-675c-43e0-b49a-6e01d1e8d135)

### 3.7 arp
    Description - Displays and modifies the IP-to-Physical(MAC) address translation tables used by
    address resolution protocol (ARP).

    Syntax - ARP -s inet_addr eth_addr [if_addr]
             ARP -d inet_addr [if_addr]
             ARP -a [inet_addr] [-N if_addr] [-v]
    Example - arp -a [Displays the ARP table, showing IP addresses mapped to MAC addresses.]
![Screenshot (563)](https://github.com/user-attachments/assets/cca5c51c-e22c-442f-9b4c-d4c296c347aa)


### 3.8 systeminfo
    Description - Displays detailed configuration information about a computer and its operating system, including 
    operating system configuration, security information, product ID, and hardware properties (such as RAM, disk space, and 
    network cards).

    Syntax - SYSTEMINFO [/S system [/U username [/P [password]]]] [/FO format] [/NH]
    Example - systeminfo
![Screenshot (568)](https://github.com/user-attachments/assets/4e83f93c-d562-4619-8779-fbc9abee6765)

### 3.9 pathping
    Description - Provides information about network latency and network loss at intermediate hops between a source and 
    destination. This command sends multiple echo Request messages to each router between a source and destination, over a 
    period of time, and then computes results based on the packets returned from each router. Because this command displays 
    the degree of packet loss at any given router or link, you can determine which routers or subnets might be having 
    network problems.

    It Combines the features of `ping` and `tracert` to identify network latency and packet loss over a route.

    Syntax -  pathping [-g host-list] [-h maximum_hops] [-i address] [-n]
                [-p period] [-q num_queries] [-w timeout]
                [-4] [-6] target_name
    Example - pathping google.com
![Screenshot (566)](https://github.com/user-attachments/assets/6e2f1e2c-1959-442b-a40f-898b1aa6a866)
It shows Hop 0 is a source with no packet loss, Hop 1 with round-time of 10ms with no packet loss and Hop 2 shows a timeout with * * * indicating that there was no response from this Hop (Router).
### 3.10 getmac
    Description -  This tool enables an administrator to display the MAC address
    for network adapters on a system.

    Syntax - GETMAC [/S system [/U username [/P [password]]]] [/FO format] [/NH] [/V]
    Example - getmac
![Screenshot (564)](https://github.com/user-attachments/assets/8feec047-3c93-4135-9a56-671441986f0c)


### 3.11 netsh
    Description - The Network Shell command-line scripting utility that allows you to, either locally or remotely, display 
    or modify the network configuration of a currently running computer. You can start this utility at the command prompt 
    or in Windows PowerShell.

    Syntax -  netsh [-a AliasFile] [-c Context] [-r RemoteMachine] [-u [DomainName\]UserName] [-p Password | *]
             [Command | -f ScriptFile]

    Example - netsh wlan show profiles
 ![Screenshot (565)](https://github.com/user-attachments/assets/f0c63189-0cb0-48a7-8940-9b97479c6642)
  
### 3.12 telnet
    Description - Allows you to connect to remote computers via the Telnet protocol. (Note: Telnet client needs to be enabled in Windows features)

    Syntax - telnet [-a][-e escape char][-f log file][-l user][-t term][host [port]]
    Example - telnet towel.blinkenlights.nl (connecting to the remote host(PC) that shows star war)



### 3.15 net use
    Description - 

    Syntax - NET USE
        [devicename | *] [\\computername\sharename[\volume] [password | *]]
        [/USER:[domainname\]username]
        [/USER:[dotted domain name\]username]
        [/USER:[username@dotted domain name]
        [/SMARTCARD]
        [/SAVECRED]
        [/REQUIREINTEGRITY]
        [/REQUIREPRIVACY]
        [/WRITETHROUGH]
        [/TRANSPORT:{TCP | QUIC} [/SKIPCERTCHECK]]
        [/REQUESTCOMPRESSION:{YES | NO}]
        [/GLOBAL]
        [[/DELETE] [/GLOBAL]]]

        NET USE {devicename | *} [password | *] /HOME

        NET USE [/PERSISTENT:{YES | NO}]

    Example -
    
### 3.16 route
    Description - Manipulates network routing tables.Displays and modifies the network routing table.

    Syntax - ROUTE [-f] [-p] [-4|-6] command [destination]
                  [MASK netmask]  [gateway] [METRIC metric]  [IF interface]
    Example - route print (prints the list of All Interfaces and the IPv4/v6 Routing Table.)
![Screenshot (598)](https://github.com/user-attachments/assets/8f6f85d5-6cd4-489a-a16e-ce86a8535609)
![Screenshot (599)](https://github.com/user-attachments/assets/3438e4f8-c7a5-4e67-addd-efd58498cb78)
![Screenshot (600)](https://github.com/user-attachments/assets/4ab93464-9ea5-443b-93d9-c973cbe0a76c)
    Example - route print 127.* (To display the routes in the IP routing table that begin with 127, type)
![Screenshot (601)](https://github.com/user-attachments/assets/ca380c72-e474-4c93-9bec-2a4e8ccec3e8)

    Syntax - route add Destination_Address 
             MASK Subnet_Mask Gateway_IP Metric

    Example -  route add 192.168.39.0 MASK 255.255.255.0 192.148.0.2
![Screenshot (603)](https://github.com/user-attachments/assets/f91c6d1d-a4c7-4d5e-9843-3ca8deb1aa4e)


### 3.17
### 3.18
### 3.19
### 3.20

## 4. Users & Groups
### 4.1 To view list of available users
    Description - net user is used to view available users in System.

    Syntax -  NET
              [ ACCOUNTS | COMPUTER | CONFIG | CONTINUE | FILE | GROUP | HELP |
              HELPMSG | LOCALGROUP | PAUSE | SESSION | SHARE | START |
              STATISTICS | STOP | TIME | USE | USER | VIEW ]
    
    Example - net /?

    Syntax - NET USER
             [username [password | *] [options]] [/DOMAIN]
             username {password | *} /ADD [options] [/DOMAIN]
             username [/DELETE] [/DOMAIN]
             username [/TIMES:{times | ALL}]
             username [/ACTIVE: {YES | NO}]
    
    Example - net user /?
    Example - net user

![Screenshot (526)](https://github.com/user-attachments/assets/5ea13a23-f886-4172-aac2-71bddc5e6e0f)
![Screenshot (527)](https://github.com/user-attachments/assets/ebd5b797-74b4-4b04-8217-be84c7dac251)

    
### 4.2 creating an user account
    Description - 
    
    Syntax - net user [username] [password] /add
    Example -
![Screenshot (528)](https://github.com/user-attachments/assets/9c74f248-877c-4ced-8740-191c8ce50495)



### 4.3 deleting user account
    Description - 

    Syntax - net user [username] /delete or del
    Example - 
![Screenshot (537)](https://github.com/user-attachments/assets/6f57030b-99f9-4da6-92a1-0ca1b475c09f)

### 4.4 enabling user account
    Description - 

    Syntax - net user [username] [/active:yes]
    Example - net user administrator /active:yes
    
![Screenshot (532)](https://github.com/user-attachments/assets/03ec5d8b-df33-4a56-bf63-7bfab8f12882)
![Screenshot (533)](https://github.com/user-attachments/assets/acd9ec04-499c-4f39-9499-c9b1fc028396)

### 4.5 disabling user account
    Description - 

    Syntax - net user [username] [/active:no]
    Example - net user administrator /active:no

![Screenshot (534)](https://github.com/user-attachments/assets/4a83b63f-6fcd-407b-bc08-9c340044ab6e)

### 4.6 changing or updating password for standard user
    Description - 
    
    Syntax - net user [username] [newpassword] or net user [username] [*]
    Example - net user ramesh 12345678
    Example - net user ramesh * [it gives us a prompt to enter new password and then confirm it.]

![Screenshot (531)](https://github.com/user-attachments/assets/60a5d104-cb15-44e0-bb59-dcc8b942a645)

### 4.7 getting detailed information about a specific user
    Description - 
    
    Syntax - net user [username]
    Example - net user ramesh
![Screenshot (529)](https://github.com/user-attachments/assets/60cff8d4-82ea-4c77-8e30-c160af16c9ee)



### 4.8 adding comment to the user
    Description -

    Syntax - net user [username] [/comment:"write comment here"]
    Example - net user ramesh /comment:"This is another user account for learning purposes"
![Screenshot (535)](https://github.com/user-attachments/assets/092a1129-eac9-4a17-85ff-4eb87ef51c29)
![Screenshot (536)](https://github.com/user-attachments/assets/606a9b63-3455-4e3a-af4f-38d1d98a947f)

### More user related commands
    Syntax - net user username /passwordchg:No or net user username /passwordchg:Yes 
    Example - net user Bolt /passwordchg:No or net user Bolt /passwordchg:Yes
![Screenshot (5711)](https://github.com/user-attachments/assets/326d5695-35bc-4691-a962-ccb6a8333efe)
![Screenshot (572)](https://github.com/user-attachments/assets/e1affdd4-471d-457a-8497-e4e9f0c62c96)

    Syntax - net user username /expires:Never or net user username /expires:MM/DD/YYYY
    Example - net user Bolt /expires:Never or net user Bolt /expires:10/10/2024
![Screenshot (573)](https://github.com/user-attachments/assets/9eb306d4-96e0-4e16-aa97-9a8301383f7b)
![Screenshot (574)](https://github.com/user-attachments/assets/5b13dec5-5f2a-4e8f-9785-b0451f2d720b)
![Screenshot (575)](https://github.com/user-attachments/assets/850c788b-4f98-48f6-b316-0b7ae95058b7)
    
    Syntax - net user [username] [/comment:"write comment here"]
    Example - net user Bolt /comment:"This is Pseudo account for practising purposes"
![Screenshot (576)](https://github.com/user-attachments/assets/431a3a2b-6845-4d24-97f5-30bf326e9038)

    Syntax - net user username /fullname:"Write Full Name"
    Example - net user Bolt /fullname:"David Bolt"
![Screenshot (577)](https://github.com/user-attachments/assets/038e6b7e-5df4-4c63-be68-1607781111bc)

    Syntax - net user username /passwordreq:No or net user username /passwordreq:Yes
    Example - net user Bolt /passwordreq:No or net user username /passwordreq:yes
![Screenshot (578)](https://github.com/user-attachments/assets/70c28fc8-ff44-4a11-a312-2b607a3abdbb)
![Screenshot (579)](https://github.com/user-attachments/assets/7b0f2d36-3a05-46d6-b23b-8ed9c5518b95)

    Syntax - net user username /times:daysofweek, time
    Example - net user Bolt /times:M-F, 09:00-18:00
![Screenshot (580)](https://github.com/user-attachments/assets/406fb05e-3427-46f7-b49c-91a5e6cd4c47)
![Screenshot (581)](https://github.com/user-attachments/assets/e08c78e5-0012-4c2d-85ec-4a46657ca712)
![Screenshot (582)](https://github.com/user-attachments/assets/5af77dee-9dec-4d56-ad50-869373413359)

    Syntax - net user username /usercomment:"write here"
    Example - net user Bolt /usercomment:"Bolt is a Team Leader"
![Screenshot (584)](https://github.com/user-attachments/assets/dbdab7b9-6979-4f44-80ee-d9dbd802dba4)

    Syntax - net user username /homedir:path
    Example - net user Bolt /times:M-F, 09:00-18:00

    Syntax - net user username /profilepath:path
    Example - net user Bolt /times:M-F, 09:00-18:00

    Synatx - net user username /scriptpath:path
    Example - net user Bolt /times:M-F, 09:00-18:00

    Syntax - net user username /addlocalgroup groupname
    Example - net user Bolt /times:M-F, 09:00-18:00

    Syntax - net user username /removelocalgroup groupname
    Example - net user Bolt /times:M-F, 09:00-18:00

    Syntax - net user username /domain
    Example - net user Bolt /times:M-F, 09:00-18:00

### 4.9 To view list of available groups
    Description -

    Syntax - net localgroup
    Example - net localgroup
![Screenshot (545)](https://github.com/user-attachments/assets/f62ac64e-f5ff-4b73-b90c-316aaf021343)
![Screenshot (542)](https://github.com/user-attachments/assets/5f0d5562-4db8-4b93-9828-5e314de27da5)
![Screenshot (543)](https://github.com/user-attachments/assets/4996c89e-78a1-4360-8ebc-b2b0252bf9ec)

### 4.10 Creating our own group
    Description -

    Syntax - net localgroup [groupname] /add
    Example - net localgroup cybersecurityteam /add
![Screenshot (546)](https://github.com/user-attachments/assets/ddfce424-b5e8-4eb9-bb68-93b6d5a9d303)


### 4.11 list members of a specific group
    Description -

    Syntax - net localgroup [groupname]
    Example - net localgroup Administrators
    Example - net localgroup cybersecurityteam
![Screenshot (544)](https://github.com/user-attachments/assets/b97e650d-127f-478b-9138-38b4894e0987)
![Screenshot (547)](https://github.com/user-attachments/assets/bd96ddf6-2816-40ac-82f4-b969b65e9a2f)

### 4.12 Updating a group
    Description -

    Syntax - net localgroup [groupname] [user] /add [it adds a new user to groups]
    Example - net localgroup cybersecurity ramesh /add 

![Screenshot (549)](https://github.com/user-attachments/assets/74c33a2f-4d2c-4c53-87d0-717253061826)

### 4.13 Deleting a group
    Description -

    Syntax - net localgroup [groupname] [user] /delete [it deletes or removes an user from group]
    Example - net localgroup cybersecurity ramesh /delete
    
    Syntax - net localgroup [groupname] /delete [it deletes a group from list of groups]
    Example - net localgroup cybersecurity /delete

![Screenshot (550)](https://github.com/user-attachments/assets/256feb40-0a17-4ede-b35d-dcbb540b31a5)
![Screenshot (551)](https://github.com/user-attachments/assets/f5626627-89ac-4fff-98e1-34a844c957cd)

### 4.14

## 5. Permission & ownerships

## 6. Process Management
### 6.1 Tasklist
### 6.2 Taskkill

## 7. Disk Space Management

## 8. Other Important commands
### 8.1 cls
    Description - Clears the terminal screen.
    
    Syntax -  
    Example - cls
    Example - help cls
    Example - cls /?
    Output -
![Screenshot (460)](https://github.com/user-attachments/assets/0e2d7c4d-7593-46d6-b5ae-a096d7893074)

![Screenshot (461)](https://github.com/user-attachments/assets/2726442f-227d-4fab-98e9-4d834b94e46f)

![Screenshot (462)](https://github.com/user-attachments/assets/b536fbd8-7c0c-41d5-a9bd-c6e141a2d463)

### 8.2
