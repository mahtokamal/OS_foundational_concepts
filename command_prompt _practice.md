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
### 3.2 ipconfig
### 3.3 nslookup
### 3.4 tracert
### 3.5 netstat
### 3.6 hostname
### 3.7 arp
### 3.8 systeminfo
### 3.9 pathping
### 3.10 getmac
### 3.11 netsh
### 3.12
### 3.15
### 3.16
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

### 4.9 To view list of available groups
    Description -

    Syntax - net user [username] [/comment:"write comment here"]
    Example - net user ramesh /comment:"This is another user account for learning purposes"
![Screenshot (542)](https://github.com/user-attachments/assets/5f0d5562-4db8-4b93-9828-5e314de27da5)
![Screenshot (543)](https://github.com/user-attachments/assets/4996c89e-78a1-4360-8ebc-b2b0252bf9ec)

### 4.10 adding our own group
### 4.11 adding user to the group

## 5. Permission & ownerships

## 6. Process Management

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
