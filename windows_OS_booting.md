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
|Active Partitions||
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




![Screenshot (374)](https://github.com/mahtokamal/OS_foundational_concepts/assets/62587491/1abe7cfd-0411-463e-a081-9ecbb4ddf9ad)

