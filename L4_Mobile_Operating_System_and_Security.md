# 1.0 Introduction

The use of mobile devices has grown very rapidly. IT technicians and professionals must be familiar with the operating systems on these devices. Like desktops and laptops, mobile devices also use operating systems to interface with the hardware and to run software. The two most commonly used mobile operating systems are Android and iOS.

In this module, you will learn about the components, functions, and terminology related to mobile operating systems. You will learn about the differences between the Android and iOS mobile operating systems, Android being open source and customizable, and iOS being proprietary to Apple and closed source. You will also learn about common mobile device features like screen orientation, screen calibration, Wi-Fi calling, virtual assistants, and GPS. You will work with both the Android and iOS operating systems as part of lab exercises.

The portable nature of mobile devices makes them at risk for theft and loss. You will learn about mobile security features such as screen lock, biometric authentication, remote lock, remote wipe, and patching and upgrading. You also learned that mobile OSs can be configured to disable access if too many failed login attempts are made. This can prevent someone from trying to guess a passcode. Most mobile devices also have a remote lock and remote wipe feature that can be activated if the device is stolen. 

# 1.1 Android versus iOS
# 1.1.1 Open Source Versus Closed Source

Like desktops and laptops, mobile devices use an operating system (OS) to run the software. This chapter focuses on the two most commonly used mobile operating systems: Android and iOS. Google develops Android, and Apple develops iOS.

Before users can analyze and modify software, they must be able to see the source code. Source code is the sequence of instructions written in human-readable language before it is turned into machine language (zeroes and ones). The source code is an essential component of free software as it allows the users to analyze and eventually modify the code. The software is said to be open source when the developer chooses to provide the source code. The software is said to be closed-source if the program’s source code is not published.

**Android GUI**

Android is an open source, Linux based smartphone/tablet operating system developed by the Open Handset Alliance, primarily driven by Google. Released in 2008 on the HTC Dream, the Android OS has been customized for use on a wide range of electronic devices. Because Android is open and customizable, programmers can use it to operate devices like laptops, smart TVs, and e-book readers. There have even been Android installations in devices like cameras, navigation systems, and portable media players. The figure shows Android running on a tablet.

![07dd20f18244c6725d16cc686264947aaf40a63d (1)](https://github.com/user-attachments/assets/9325c366-cfcb-435c-888e-3266f42cb834)

**iOS GUI**

iOS is a closed source Unix based operating system for Apple’s iPhone smartphone and iPad tablet. Released in 2007 on the first iPhone, the Apple iOS source code was not released to the public. To copy, modify or redistribute iOS requires permission from Apple. The figure shows iOS running on an iPhone.

![5a9604def55d1862c199ddbb1d23ae601e204788](https://github.com/user-attachments/assets/df313792-6ab5-4c81-bd38-ccceeae9f59a)

**Windows 10 Mobile**

iOS is not the only closed source OS for mobile devices. Microsoft also created a version of Windows for their mobile devices. This includes Windows CE, Windows Phone 7, shown in the figure, and Windows Phone 8. With the development of Windows 10 Mobile, Microsoft provides a very similar user interface and use of code an all of their devices. This includes their Windows 10 Mobile phones and tablets they develop under the name Surface.

![ab5f5ff91e50c452e368b9577b7e3846ceb065fe](https://github.com/user-attachments/assets/915fc555-4678-49f5-9711-5db0796cc1ef)

# 1.1.2 Application and Content Sources

Apps are programs that are executed on mobile devices. Apps are written and compiled for a specific mobile operating system such as Apple iOS, Android, or Windows. Mobile devices come with several different apps preinstalled to provide basic functionality. There are apps to make phone calls, send and receive an email, listen to music, take pictures, and play video or video games.
Apps are used on mobile devices in the same way programs are used on computers. Instead of being installed from an optical disk, apps are downloaded from a content source. Some apps can be downloaded for free, and others must be purchased.

**iOS Apps**

Apps for Apple iOS mobile devices are available for free or purchase from the App Store. Apple uses a walled garden model for their apps meaning the apps must be submitted to and approved by Apple before they are released to users. This helps prevent the spread of malware and malicious code. Third-party developers can create apps for iOS devices by using Apple’s Software Development Kit (SDK) Xcode and the Swift programming language. Note that Xcode can only be installed on computers running OS X.

![3bc49aa07fb4058369a5515f99dceb9276d95852](https://github.com/user-attachments/assets/7126b4f0-46c0-482e-9d01-8bfa9ccf7938)

**Android Apps**

Android apps are available from both Google PlayTM and third-party sites, such as Amazon’s App store. Android Studio, a Java-based SDK, is available on Linux, Windows, and OS X. Android apps run in a sandbox and have only the privileges enabled by the user. A prompt will appear if an app needs to obtain permissions. Permissions are granted via the app’s Settings page.
Third-party or custom programs are installed directly using an Android Application Package (apk) file. This gives users the ability to directly install apps without going through the storefront interface. This is known as sideloading. Click each image below for more information on apps.

![04b80822bd511934c01caae8d2c397feca9fefb3](https://github.com/user-attachments/assets/c22fc9ef-ebf7-4a06-954a-723b16711531)

**Automobile Apps**

Many new cars have navigation built into them. Some also have what is known as in-vehicle entertainment systems. A growing trend is using many apps on your mobile device through this entertainment system. Your tablet or smartphone is connected to the system via USB or Bluetooth to enable what is known as Android Auto or Apple CarPlay. Navigation is one of the most common uses for this connection. You can also access the music on your mobile device and play it over the car stereo. Other features include talk-to-text, hands-free calling, access to digital assistants, and a display of your calendar contents.

# 1.1.3 Quiz

# 1.2 Mobile Touch Inteface
# 1.2.1 Android Home Screen Items

Much like a desktop or laptop computer, mobile devices organize icons and widgets on multiple screens for easy access.

**Android Main Home Screen**

One screen is designated as the home screen. Additional screens are accessed by sliding the home screen to the left or right. Each screen contains navigation icons, the main area where icons and widgets are accessed, and notification and system icons. The screen indicator displays which screen is currently active.

![07dd20f18244c6725d16cc686264947aaf40a63d](https://github.com/user-attachments/assets/b10040b7-5cb9-47e9-a81a-8ffa5d8149b4)

**Navigation Icons**

The Android OS uses the system bar to navigate apps and screens. The system bar is always displayed at the bottom of every screen.

![f3c452a958df5e627e595511daf26ce9f4f1b50c](https://github.com/user-attachments/assets/b5791846-dcd3-4ac8-a0ca-cbb7edc8a586)

**Notification and System Icons**

Each Android device has an area that contains system icons, such as the clock, battery status, and radio signal status for Wi-Fi and provider networks. Apps such as email, text messaging, and Facebook often display status icons to indicate communication activity.

To open the notification area on Android devices, swipe down from the top of the screen. You can do the following when notifications are open:

- Respond to a notification by touching it.
- Dismiss a notification by swiping it off the screen to either side.
- Dismiss all notifications with the icon.
- Toggle often-used settings.
- Adjust the brightness of the screen.
- Open the Settings menu with the quick settings icon.
- The Android OS uses the system bar to navigate apps and screens. The system bar is always displayed at the bottom of every screen.

![4fa0ae585bdb7dcbe6eb32252e8ea30ea879c95b](https://github.com/user-attachments/assets/5b3f59b8-b4ea-426c-a313-4def45fd2fcc)

# 1.2.2 Lab - Working with Android

# 1.2.3 iOS Home Screen Items

The iOS interface works in much the same way as the Android interface. Screens are used to organize apps launched with a touch. There are some significant differences:

- No navigation icons - A physical button may be pressed instead of touching navigation icons.
- No widgets - Only apps and other content can be installed on iOS device screens.
- No app shortcuts - Each app on a home screen is the actual app, not a shortcut.

**Home button**

Unlike Android, iOS devices do not use navigation icons to perform functions. On iPhone versions prior to the iPhone X, a single physical button called the Home button performs many of the same functions as the Android navigation buttons. For these older phones, the Home button is at the bottom of the device and can perform many functions. Some common functions performed by the home button with explanations of how these functions are performed on the iPhone X, which has eliminated the home button, are shown below:

![24934774699e310a4e1567e8aec3175b4167b9d0](https://github.com/user-attachments/assets/6f0deed0-f9c1-4699-8c74-986044d3c885)

**Wake the device** - When the device’s screen is off, press the Home button once to turn it on. On iPhone X you can wake the device using either facial recognition or by raising the phone and tapping the screen. (Raise to wake is also available on iPhone versions 6s or later.)

**Return to the home screen** - Press the Home button while using an app to return to the last home screen that was used. On iPhone X return to the home screen by swiping the screen up from the bottom.

**Start Siri or voice control** – Press and hold the Home button to start Siri or voice control. Siri is special software that understands advanced voice controls. On iPhone X Siri is launched by pressing and holding the side button.

**iOS Notification Center**

iOS devices have a notification center that displays all alerts in one location. To open the notification area on iOS devices, touch the top center of the screen and swipe down. This will show the phone's lock screen. Any notifications will appear in the middle area of the screen, as shown in the figure. From here, you can browse notifications and alerts, dismiss them, clear them, and adjust them as necessary.

![7dadf2598817062c95998b8e74f4dad2bed4d5a5](https://github.com/user-attachments/assets/5d9ea96f-2ffd-4914-ab56-7b791085c4c4)

**Commonly Used Settings**

iOS devices allow the user to quickly access common settings and switches, even if the device is locked. To access the commonly used settings menu, swipe down from the top right corner.

The Control Center comes with some default controls that are always available. You can configure addition controls by navigating to **Settings > Control Center**. In the figure, the user has added the Flashlight, Timer, Calculator, Camera, and other apps to the Control Center screen.

![6ab866f8f4510dd4368853a5b86a70e8ef6fe88c](https://github.com/user-attachments/assets/7b04ed08-132b-44b7-8da9-0912e6306386)

**iOS Spotlight**

From any screen of an iOS device, touch the screen and drag down to reveal the Spotlight search field. Any part of the screen except the very top or the very bottom should work. When Spotlight search field is revealed, type what you're looking for. Spotlight shows suggestions from many sources including your installed apps, Setting, the internet, iTunes, App Store, movie show times, and nearby locations. Spotlight also automatically updates the results as you type.

![9f2be4bcf41ca574882f60a000fbb3add61a0219](https://github.com/user-attachments/assets/0c8ff982-9608-46d5-b25f-7e670d233ff2)

# 1.2.4 Lab - Working with iOS

# 1.3 Common Mobile Device Features
# 1.3.1 Screen Orientation

Most mobile devices function in either portrait or landscape mode. A sensor inside the device, known as an accelerometer, detects how it is being held and will change the screen orientation appropriately. Users can choose the viewing mode that is the most comfortable for them for different types of content or applications. Content rotates to the position of the device. This feature is useful, for example, when taking a photograph. The camera app also turns to landscape mode when the device turns to landscape mode. Also, when a user writes a text, turning the device to landscape mode makes the keyboard larger and broader.

Some devices have gyroscopes to provide more accurate movement readings. Gyroscopes allows a control mechanism for driving games where the phone or tablet functions as a steering wheel.

**Android Screen Auto-Rotation Setting**

When using an Android device, to enable auto rotation, open the notifications panel and turn on the auto-rotate function by tapping the screen rotation icon, indicated in the figure.

![580ea56cd43fe4635a6851c197ca318bcff23728](https://github.com/user-attachments/assets/9f1b9305-7204-4e3a-a207-7984a2e3e2d9)

**iOS Screen Auto-Rotation Setting**

When using an iOS device, to enable automatic rotation use the following procedure:
Swipe down from the top right corner to open the Control Center, and tap the lock icon, as shown in the figure.

![9c5cfe68ad5a2adde5e71cbd95d53110cd996131](https://github.com/user-attachments/assets/aad77781-3b42-4744-8baa-5705e68a68e8)

# 1.3.2 Screen Calibration

You may need to adjust the screen's brightness when using a mobile device. When bright sunlight makes the screen difficult to read, increase the brightness level. Inversely, very low brightness is helpful when reading a book on a mobile device at night. Mobile devices can auto-adjust the brightness depending on the amount of surrounding light. The device must have a light sensor to use auto-brightness.

The LCD screen for most mobile devices uses the most battery power. Lowering the brightness or using auto-brightness helps conserve battery power. Set the brightness to the lowest to get the device the most battery life.

**Android Brightness Menu**

When using an Android device, to configure screen brightness use the following path:

**Swipe down from the very top of the screen > Display > Brightness > slide the brightness to the desired level**

Alternatively, tap the **Adaptive Brightness** toggle to allow the device to decide the optimal screen brightness based on the amount of ambient light.

![537cedbd5f3a7cef06d6d1ddb516ab8c8738aad6](https://github.com/user-attachments/assets/ae3307b4-e551-4ad2-8097-08a3a441a7f4)

**iOS Display & Brightness Menu**

When using an iOS device, to configure screen brightness, use the following path:

Swipe down from the top right corner and slide the brightness bar up or down to vary the brightness.

Alternatively, to configure brightness in the Settings menu, use the following path:
**Settings > Display & Brightness > slide the brightness to the desired level.**

![4363291a3b4d2c206e27c01d556599ae845c5f4e](https://github.com/user-attachments/assets/1ea2a841-b665-4906-bcf2-a2b0fad1974c)

# 1.3.3 GPS

Another common feature of mobile devices is the Global Positioning System (GPS). GPS is a navigation system that determines the time and geographical location of the device by using messages from satellites in space and a receiver on Earth. A GPS radio receiver uses at least four satellites to calculate its position based on the messages. GPS is very accurate, even used under most weather conditions. However, dense foliage, tunnels, and tall buildings can interrupt satellite signals. GPS receivers must have line-of-sight to GPS satellites and do not work indoors. Indoor Positioning Systems (IPS) can determine device location by triangulating its proximity to other radio signals, such as Wi-Fi access points.

GPS services allow app vendors and websites to know a device's location and offer location-specific services (such as local weather and advertising). This is called geotracking.

**Android Location Services**

To enable GPS on Android devices use the following path:

**Settings > Location > Tap on the toggle to turn location services on**

![13e55cfaa35862001811e76993f5914b19081f35](https://github.com/user-attachments/assets/b98aba17-5c88-42a8-9fc4-e874bcdd2c83)

**iOS Location Services**

To enable GPS on iOS devices use the following path:

**Settings > Privacy & Security > Location Services > Turn location services on**

![99f22320775de799385bfcf943792dcc4ff8646a](https://github.com/user-attachments/assets/b9538afb-a4ca-445e-9175-244013b6cfef)

# 1.3.4 Lab - Mobile Device Features
# 1.3.5 Wi-Fi Calling

Instead of using the cellular carrier's network, modern smartphones can use the internet to transport voice calls by taking advantage of a local Wi-Fi hotspot. This is called Wi-Fi calling. Locations such as coffee shops, workplaces, libraries, or homes, usually have Wi-Fi networks connected to the internet. The phone can transport voice calls through the local Wi-Fi hotspot. If there is no Wi-Fi hotspot within reach, the phone will use the cellular carrier's network to transport voice calls.

Wi-Fi calling is beneficial in areas with poor cellular coverage because it uses a local Wi-Fi hotspot to fill the gaps. The Wi-Fi hotspot must guarantee a throughput of at least 1Mbps to the internet for a good quality call. When Wi-Fi calling is enabled and used during a voice call, the phone will display "Wi-Fi" next to the carrier name.

**Enabling Wi-Fi Calling on Android**

To enable Wi-Fi calling on Android use the following path:

**Settings > More (under Wireless & networks section) > Wi-Fi Calling > Tap on the toggle to turn it on**

![e81a722e5fcd2c8840da24d88fabed3194556dc0](https://github.com/user-attachments/assets/2ac63a56-9c00-410b-bac8-5315379af6de)

**Enabling Wi-Fi Calling on iOS**

To enable Wi-Fi calling on iOS use the following path:

**Settings > Wi-Fi and turn on Wi-Fi Calling**

![85e78ff87ac58423fd636d3d80457b0df65176c2](https://github.com/user-attachments/assets/b89961f9-cafc-4cf6-983e-2f2be1a6265a)

**Note:** Not all cellular carriers allow Wi-Fi calling. If you cannot enable it on your phone, your carrier or mobile device probably does not support it.

# 1.3.6 Mobile Payments

Mobile payments refer to any payments made through a mobile phone.

**1. Premium SMS Based Transactional Payments**

**Premium SMS Based Transactional Payments**

Consumers send an SMS message to a carrier's special phone number containing a payment request. The seller is informed the payment has been received and is cleared to release the goods. The charge is then added to the customer's phone bill. Slow speed, poor reliability, and poor security are a few shortcomings of this method.

**2. Direct Mobile Billing**
**Direct Mobile Billing**

Using a mobile billing option during check-out, a user identifies their self (usually through two-factor authentication) and allows the charge to be added to the mobile service bill. This is very popular in Asia and has the following benefits: security, convenience, and no need for bank cards or credit cards.

**3. Mobile Web Payments Contactless**
**Mobile Web Payments Contactless**

The consumer uses the web or dedicated apps to complete the transaction. This method relies on the Wireless Application Protocol (WAP) and usually requires the use of credit cards or a pre-registered online payment solution, such as PayPal or Venmo.

**4. Contactless NFC**
**Contactless NFC**

Near Field Communication (NFC) is a mobile payment method used mostly in physical store transactions. A consumer pays for good or services by waving the phone near the payment system. Based on a unique ID, the payment is charged directly against a pre-paid account or bank account. NFC is also used in mass-transportation services, the public parking sector, and many other consumer areas.

# 1.3.7 Virtual Private Network

A Virtual Private Network (VPN) is a private network that uses a public network (usually the internet) to connect remote sites or users. Instead of a dedicated leased line, a VPN uses "virtual" connections routed through the internet from the company's private network to the remote site or employee.

Many companies create their VPNs to accommodate the needs of remote employees and distant offices. With the proliferation of mobile devices, it was a natural move to add VPN clients to smartphones and tablets.

For a VPN established from a client to a server, the client accesses the network behind the server like it was connected directly to that network. Because VPN protocols also allow for data encryption, the communication between client and server is secure.

When the device has VPN information loaded, that device must start before traffic can be sent and received.

**Configuring a VPN Connection on Android**

To create a new VPN connection on Android use the following path:

![7f4c46c87507a5f4108f837724d375fdecf30b17](https://github.com/user-attachments/assets/0572a3ac-7605-4fbb-b503-5673e6b9c378)

**Settings > More (under Wireless & networks section) > VPN > Tap on the + sign to add a VPN connection**

**Starting a VPN Connection on Android**

To start a VPN on Android use the following path:

![add444a72beec6b2c5a5e7f2ead359e70cd717f6](https://github.com/user-attachments/assets/e4b0dd48-d80e-42cc-b899-b2b4aabfce71)

**Settings > General > VPN > Select the desired VPN connection > enter username and password > tap CONNECT**

**Configuring a VPN Connection on iOS**

To create a new VPN connection on iOS use the following path:

![64440c07db5a690d363e19c2d11260dd9ff4255e](https://github.com/user-attachments/assets/851f6b44-20fe-432b-8e70-308205cf0c54)

**Settings > General > VPN > Add VPN Configuration...**

**Starting a VPN Connection on iOS**

To start a VPN on iOS use the following path:

![26330611d4d87425183b3c5408856195c086b612](https://github.com/user-attachments/assets/fcc4d467-ed27-4e61-947b-45f30df6c9fb)

**Settings > Toggle VPN to on**

# 1.3.8 Virtual Assistants

A digital assistant sometimes called a virtual assistant, is a program that can understand natural conversational language and perform tasks for the end user. Modern mobile devices are powerful computers, making them the perfect platform for digital assistants. Popular digital assistants include Google Now for Android, Siri for iOS, and Cortana for Windows Phone.

These digital assistants rely on artificial intelligence, machine learning, and voice recognition technology to understand conversational-style voice commands. As the end user interacts with these digital assistants, sophisticated algorithms predict the user's needs and fulfill requests. By pairing simple voice requests with other inputs, such as GPS location, these assistants can perform several tasks, including playing a specific song, performing a web search, taking a note, or sending an email.

**Google Now**

To access Google Now on an Android device simply say "Okay google" and Google Now will activate and start listening to requests.

![e14cf2b7a89647c0444b75f0cba66c65e247dadf](https://github.com/user-attachments/assets/4e496802-61ce-40ea-ac70-499daa3cc769)

**iOS Display & Brightness Menu**

To access Siri on an iOS device, press and hold the Home button. Siri will activate and start listening to requests. Alternatively, Siri can be configured to start listening to commands when it hears "Hey Siri". To enable "Hey Siri", use the following path:

**Settings > Siri & Search > Toggle Listen for "Hey Siri".**

In the figure, Siri has responded to the user's request for a weather forecast.

![1ea542af4c4ae040621844a5d254288e35c60485](https://github.com/user-attachments/assets/075832c5-bf22-413d-acd4-ef740b32ba50)

# 1.4 Passcode Locks
# 1.4.1 What do you already know? - Screen Locks
# 1.4.2 Lab - passcodes Locks
# 1.4.3 Restrictions on Failed Login Attempts

Unlocking a mobile device requires entering the correct PIN, password, pattern, or another passcode type. In theory, a passcode, such as a PIN, could be guessed given enough time and perseverance. Mobile devices can perform defined actions after incorrect attempts to prevent someone from trying to guess a passcode.

For Android devices, the number of failed attempts before lockout depends on the device and version of Android OS. Commonly, an Android device will lock when a passcode has failed from 4 to 12 times. After a device is locked, you can unlock it by entering the Gmail account information used to set up the device.

**iOS Erase Data**

For iOS devices, you can turn on the Erase data option as shown. If the passcode fails 10 times, the screen goes black, and all data on the device is deleted. To restore the iOS device and data, if you have backups, use either the Restore and Backup option in iTunes or the Manage Storage option in iCloud.

**Note:** The iPhone in the figure is managed by Cisco. As part of Cisco's security policy, the user is not allowed to turn off **Erase Data.** Therefore, if the wrong password is entered 10 times, all data will be erased.

![a8c344d87925ceed14be8b298b566b6e28d82a9f](https://github.com/user-attachments/assets/3333c42c-c973-46dd-bff9-ef9c757bf209)

**iOS GUI**

On iOS, to increase security, the passcode is used as part of the encryption key for the entire system. Because the passcode is not stored anywhere, no one can gain access to the user data on iOS devices, including Apple. The system depends on the user to provide the passcode before the system can be unlocked and decrypted for use. A forgotten passcode will render user data unreachable, forcing the user to perform a full restore from a backup saved in iTunes or iCloud.

![3407d9504aabde5fa495c944cc166521233681f6](https://github.com/user-attachments/assets/c451f86b-3e73-4516-ac8b-9cc9fcc3b1b0)

# 1.4.4 Check Your Understanding - Screen Locks and Biometric Authentications

# 1.5 Cloud-Enabled Services for Mobile Devices
# 1.5.1 Remote Backup

Mobile device data can be lost due to device failures or the loss or theft of the device. Periodically back up data to ensure it is recoverable if needed. With mobile devices, storage is often limited and not removable. Perform remote backups to overcome these limitations. A remote backup is when a device copies its data to cloud storage using a backup app. To restore data, run the backup app and access the website to retrieve the data.

Most mobile operating systems have a user account linked to the vendor’s cloud services, such as iCloud for iOS, Google Sync for Android, and OneDrive for Microsoft. The user can enable automatic backups to the cloud for data, apps, and settings. Some third-party backup providers, such as Dropbox, can be used. Mobile devices can back up to a PC. iOS supports backups on iTunes running on a PC. Another option is configuring Mobile Device Management (MDM) software to back up user devices automatically.

![9c06f2333eab96abd2c98e3e8120ff3a370e440b](https://github.com/user-attachments/assets/c9d9b230-7fa6-4a1f-ba1a-6999a8d77b67)

# 1.5.2 Locator Applications

If a mobile device is misplaced or stolen, it is possible to find it using a locator app. A locator app should be installed and configured on each mobile device before it is lost. Both Android and iOS have apps for remotely locating a device.

Like Apple’s Find My iPhone, Google Find My Device allows a user to locate, ring, or lock a lost Android device or erase data from the device. To manage a lost device, the user must visit Google Find My Device hosted at https://www.google.com/android/find and log in with the Google account used on the Android device. Google Find My Device is included and enabled by default on Android 5. x and can be found under **Settings > Biometrics Security > Find My Mobile.**

iOS users can use the Find My iPhone app, as shown in the figure. The first step is to install the app, start it, and follow the instructions to configure the software. Different iOS devices locate a lost device with The Find My iPhone app.

<img width="745" alt="89abd0d93282645d66b646fc7a176b452432a07a" src="https://github.com/user-attachments/assets/efc33650-ddde-498f-9443-33d3e49031d5">

**Note:** If the app cannot locate the lost device, the device might be turned off or disconnected. Connect to a cellular or wireless network to receive app commands or send location information to the user.

After locating the device, you might be able to perform additional functions, such as sending a message or playing a sound. These options are helpful if you have misplaced your device. If the device is close by, playing a sound indicates the location. If the device is at another site, sending a message to display on the screen allows the finder to contact you. 

# 1.5.3 Remote Lock and Remote Wipe

If attempts to locate a mobile device have failed, other security features can prevent data on the device from being compromised. Usually, the same apps that perform remote locations have security features. Two of the most common security features are remote lock and wipe.

**Note:** For these remote security measures to function, the device must be powered on and connected to a cellular or Wi-Fi network.

**Remote Lock**

The remote lock feature for iOS devices is called lost mode. The Android Device Manager calls this feature Lock. It allows you to lock the device with a passcode, so others cannot gain access to the data in the device. For example, the user can display custom messages, or keep the phone from ringing due to incoming calls or text messages.

<img width="745" alt="125f6d22feaf570bd0b88b9529a026802c92eab6" src="https://github.com/user-attachments/assets/fc919c80-6797-4a01-b68a-9f57060e57bd">

**Remote Wipe**

The remote wipe feature for iOS devices is called erase phone. The Android Device Manager calls this feature Erase. It deletes all data from the device and returns it to a factory state. To restore data to the device, Android users must set up the device using a Gmail account, and iOS users must synchronize their device to iTunes.

Most mobile device operating systems provide a full device encryption feature. Full device encryption can prevent anyone in possession of the device from circumventing the device’s access controls and reading the raw data stored in memory.

All user data on an iOS device is always encrypted and the key is stored on the device. When used to “wipe” the device, the OS deletes the key, and the data becomes inaccessible. Data Protection encryption is enabled automatically when a password lock is configured on the device.

On Android OS, encryption is enabled through **Settings > Security.** Android uses full-disk encryption with a passcode-derived key.

<img width="745" alt="65b5b5c773b15bb4c4481c625396458e76e05076" src="https://github.com/user-attachments/assets/54debd6c-05a1-445e-a6b3-0330dca4c287">

# 1.5.4 Check Your Understanding - Cloud - Enabled Services for Mobile Devices

# 1.6 Mobile Device Software Security
# 1.6.1 Antivirus

All computers are vulnerable to malicious software. Smartphones and other mobile devices are computers and are also vulnerable. Antivirus apps are available for both Android and iOS. Depending on the permissions granted to antivirus apps when installed on an Android device, the app might not be able to scan files automatically or run scheduled scans. Manually initiate file scans. iOS does not allow automatic or scheduled scans. This safety feature prevents malicious programs from using unauthorized resources or contaminating other apps or the OS. Some antivirus apps also provide locator services, remote lock, or remote wipe.

Mobile device apps run in a sandbox. A sandbox is a location of the OS that keeps code isolated from other resources and other code. It is difficult for malicious programs to infect a mobile device because apps run inside the sandbox. An Android app asks for permission to access specific resources upon installation. A malicious app can access any resources that were allowed permission during installation. This is another reason why it is vital to download apps only from trusted sources. A trusted app source is authenticated and authorized by a service provider. The service provider issues the developer a certificate to sign their apps and identify them as trusted.

Due to the nature of the sandbox, malicious software does not usually damage mobile devices; it is far more likely for a mobile device to transfer a malicious program to another device, such as a laptop or desktop. For example, suppose a malicious program download from email, the Internet, or another device. In that case, a malicious program can be placed on a laptop the next time it connects to a mobile device.

To prevent the malicious program from infecting additional devices, use a firewall. Firewall apps for mobile devices can Monitor app activity and prevent connections to specific ports or IP addresses. Because mobile device firewalls must be able to control other apps, they logically work at a higher (root) permission level. No root firewalls work by creating a virtual private network (VPN) and then controlling app access to the VPN.

![1ec2ff28bc87a2c3a3b2a798406e9dfb750d8a10](https://github.com/user-attachments/assets/fd47223e-bcda-4ea1-819b-f2d2f0cf6b3a)

# 1.6.2 Rooting and jailbreaking

Several software restrictions usually protect mobile operating systems. For example, an unmodified copy of iOS will only execute authorized code and allow minimal user access to its file system.

Rooting and Jailbreaking are two methods for removing restrictions and protections added to mobile operating systems. They are a means of circumventing the usual operating of the device operating system to gain super-user or root administrator permissions. Rooting is used on Android devices to gain privileged or root-level access for modifying code or installing software not intended for the device. Jailbreaking is typically used on iOS devices to remove manufacturer restrictions allowing them to run arbitrary user code and granting users full access to the file system and kernel modules.

Rooting or jailbreaking a mobile device usually voids the manufacturer's warranty. Although modifications are discouraged, a large group of users choose to remove their own devices' restrictions. Rooting or jailbreaking a mobile device customizes the GUI to improve the speed and responsiveness of the device. Apps come from secondary or unsupported sources.

Jailbreaking exploits vulnerabilities in iOS. A program is written after finding a usable vulnerability. This program is the actual jailbreak software distributed on the internet. Apple discourages jailbreaking and actively works towards eliminating vulnerabilities that make jailbreaking possible on iOS. In addition to the OS updates and bug fixes, new iOS releases usually include patches to eliminate known vulnerabilities that allow jailbreaking. When updates fix iOS vulnerabilities, it forces hackers to start over.

**Note:** The jailbreak process is completely reversible. To remove the jailbreak and bring the device back to its factory state, connect it to iTunes and perform a Restore.

![04d4a5ba885748badb498a928e631ac1819d7d7f](https://github.com/user-attachments/assets/c9d8a1f7-b2b5-4f67-bd87-cbe1c9d87875)

# 1.6.3 Patching and Updating Operating Systems

You can update or patch the OS on mobile devices like the OS on a desktop or laptop. Updates add functionality or increase performance. Patches can fix security problems or issues with hardware and software.

Because there are so many Android mobile devices, updates and patches do not release as one package for all devices. Sometimes a new version of Android cannot install on older devices where the hardware does not meet the minimum specifications. These devices might receive patches to fix known issues but not receive OS upgrades.

Android updates and patches use an automated process for delivery. When a carrier or manufacturer has an update for a device, a notification on the device indicates that an update is ready. Touch the update to begin the download and installation process.

iOS updates use an automated process for delivery. Devices that do not meet the hardware requirements are excluded. The easiest method to check for iOS updates is on the iPhone, go to **Settings > General > Software Update**, as shown in the figure.

![1e6b0dbef538995b230450fe2c5de0f1f402339a](https://github.com/user-attachments/assets/17d2fd47-45b4-433c-95e7-8b9550f54ce4)

Two other types of updates for mobile device radio firmware are important. These are called baseband updates and consist of the Preferred Roaming List (PRL) and the Primary Rate ISDN (PRI). The PRL is configuration information that a cellular phone needs to communicate on other networks to call outside the carrier’s network. The PRI configures the data rates between the device and the cell tower. This ensures that the device can communicate with the tower at the correct rate.

# 1.6.4 Check Your Understanding - Mobile Device Software Security

# 1.7 Mobile Operating Systems and Security Summary
# 1.7.1 What Did I learn in this Module?
**1. Android Versus iOS**

**Topic Objective:** Compare the Android and iOS operating systems.

**2. Mobile Touch Interface**

**Topic Objective:** Describe the features of the Android and iOS touch interfaces.

**3. Common Mobile Device features**

**Topic Objective:** Describe operating system features that are common among mobile devices.

**4. Passcode Locks**

**Topic Objective:** Explain how to configure various types of passcode locks.

**5. Cloud-Enabled Services for Mobile Devices**

**Topic Objective:** Describe Cloud-enabled services for mobile devices.

**6. Mobile Device Software Security**

**Topic Objective:** Describe software security for mobile devices.

# 1.7.2 Quiz - Mobile Operating Systems and Security

