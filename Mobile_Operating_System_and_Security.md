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

**iOS GUI**

iOS is a closed source Unix based operating system for Apple’s iPhone smartphone and iPad tablet. Released in 2007 on the first iPhone, the Apple iOS source code was not released to the public. To copy, modify or redistribute iOS requires permission from Apple. The figure shows iOS running on an iPhone.

**Windows 10 Mobile**

iOS is not the only closed source OS for mobile devices. Microsoft also created a version of Windows for their mobile devices. This includes Windows CE, Windows Phone 7, shown in the figure, and Windows Phone 8. With the development of Windows 10 Mobile, Microsoft provides a very similar user interface and use of code an all of their devices. This includes their Windows 10 Mobile phones and tablets they develop under the name Surface.

# 1.1.2 Application and Content Sources

Apps are programs that are executed on mobile devices. Apps are written and compiled for a specific mobile operating system such as Apple iOS, Android, or Windows. Mobile devices come with several different apps preinstalled to provide basic functionality. There are apps to make phone calls, send and receive an email, listen to music, take pictures, and play video or video games.
Apps are used on mobile devices in the same way programs are used on computers. Instead of being installed from an optical disk, apps are downloaded from a content source. Some apps can be downloaded for free, and others must be purchased.

**iOS Apps**

Apps for Apple iOS mobile devices are available for free or purchase from the App Store. Apple uses a walled garden model for their apps meaning the apps must be submitted to and approved by Apple before they are released to users. This helps prevent the spread of malware and malicious code. Third-party developers can create apps for iOS devices by using Apple’s Software Development Kit (SDK) Xcode and the Swift programming language. Note that Xcode can only be installed on computers running OS X.

**Android Apps**

Android apps are available from both Google PlayTM and third-party sites, such as Amazon’s App store. Android Studio, a Java-based SDK, is available on Linux, Windows, and OS X. Android apps run in a sandbox and have only the privileges enabled by the user. A prompt will appear if an app needs to obtain permissions. Permissions are granted via the app’s Settings page.
Third-party or custom programs are installed directly using an Android Application Package (apk) file. This gives users the ability to directly install apps without going through the storefront interface. This is known as sideloading. Click each image below for more information on apps.

**Automobile Apps**

Many new cars have navigation built into them. Some also have what is known as in-vehicle entertainment systems. A growing trend is using many apps on your mobile device through this entertainment system. Your tablet or smartphone is connected to the system via USB or Bluetooth to enable what is known as Android Auto or Apple CarPlay. Navigation is one of the most common uses for this connection. You can also access the music on your mobile device and play it over the car stereo. Other features include talk-to-text, hands-free calling, access to digital assistants, and a display of your calendar contents.

# 1.1.3 Quiz

# 1.2 Mobile Touch Inteface
# 1.2.1 Android Home Screen Items

Much like a desktop or laptop computer, mobile devices organize icons and widgets on multiple screens for easy access.

**Android Main Home Screen**

One screen is designated as the home screen. Additional screens are accessed by sliding the home screen to the left or right. Each screen contains navigation icons, the main area where icons and widgets are accessed, and notification and system icons. The screen indicator displays which screen is currently active.

**Navigation Icons**

The Android OS uses the system bar to navigate apps and screens. The system bar is always displayed at the bottom of every screen.

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

# 1.2.2 Lab - Working with Android
# 1.2.3 iOS Home Screen Items

The iOS interface works in much the same way as the Android interface. Screens are used to organize apps launched with a touch. There are some significant differences:

- No navigation icons - A physical button may be pressed instead of touching navigation icons.
- No widgets - Only apps and other content can be installed on iOS device screens.
- No app shortcuts - Each app on a home screen is the actual app, not a shortcut.

**Home button**

Unlike Android, iOS devices do not use navigation icons to perform functions. On iPhone versions prior to the iPhone X, a single physical button called the Home button performs many of the same functions as the Android navigation buttons. For these older phones, the Home button is at the bottom of the device and can perform many functions. Some common functions performed by the home button with explanations of how these functions are performed on the iPhone X, which has eliminated the home button, are shown below:

Wake the device - When the device’s screen is off, press the Home button once to turn it on. On iPhone X you can wake the device using either facial recognition or by raising the phone and tapping the screen. (Raise to wake is also available on iPhone versions 6s or later.)
Return to the home screen - Press the Home button while using an app to return to the last home screen that was used. On iPhone X return to the home screen by swiping the screen up from the bottom.
Start Siri or voice control – Press and hold the Home button to start Siri or voice control. Siri is special software that understands advanced voice controls. On iPhone X Siri is launched by pressing and holding the side button.

**iOS Notification Center**

iOS devices have a notification center that displays all alerts in one location. To open the notification area on iOS devices, touch the top center of the screen and swipe down. This will show the phone's lock screen. Any notifications will appear in the middle area of the screen, as shown in the figure. From here, you can browse notifications and alerts, dismiss them, clear them, and adjust them as necessary.

**Commonly Used Settings**

iOS devices allow the user to quickly access common settings and switches, even if the device is locked. To access the commonly used settings menu, swipe down from the top right corner.

The Control Center comes with some default controls that are always available. You can configure addition controls by navigating to Settings > Control Center. In the figure, the user has added the Flashlight, Timer, Calculator, Camera, and other apps to the Control Center screen.

**iOS Spotlight**

From any screen of an iOS device, touch the screen and drag down to reveal the Spotlight search field. Any part of the screen except the very top or the very bottom should work. When Spotlight search field is revealed, type what you're looking for. Spotlight shows suggestions from many sources including your installed apps, Setting, the internet, iTunes, App Store, movie show times, and nearby locations. Spotlight also automatically updates the results as you type.

# 1.2.4 Lab - Working with iOS

# 1.3 Common Mobile Device Features
# 1.3.1 Screen Orientation

Most mobile devices function in either portrait or landscape mode. A sensor inside the device, known as an accelerometer, detects how it is being held and will change the screen orientation appropriately. Users can choose the viewing mode that is the most comfortable for them for different types of content or applications. Content rotates to the position of the device. This feature is useful, for example, when taking a photograph. The camera app also turns to landscape mode when the device turns to landscape mode. Also, when a user writes a text, turning the device to landscape mode makes the keyboard larger and broader.

Some devices have gyroscopes to provide more accurate movement readings. Gyroscopes allows a control mechanism for driving games where the phone or tablet functions as a steering wheel.

**Android Screen Auto-Rotation Setting**

When using an Android device, to enable auto rotation, open the notifications panel and turn on the auto-rotate function by tapping the screen rotation icon, indicated in the figure.

**iOS Screen Auto-Rotation Setting**

When using an iOS device, to enable automatic rotation use the following procedure:
Swipe down from the top right corner to open the Control Center, and tap the lock icon, as shown in the figure.

# 1.3.2 Screen Calibration

You may need to adjust the screen's brightness when using a mobile device. When bright sunlight makes the screen difficult to read, increase the brightness level. Inversely, very low brightness is helpful when reading a book on a mobile device at night. Mobile devices can auto-adjust the brightness depending on the amount of surrounding light. The device must have a light sensor to use auto-brightness.

The LCD screen for most mobile devices uses the most battery power. Lowering the brightness or using auto-brightness helps conserve battery power. Set the brightness to the lowest to get the device the most battery life.

**Android Brightness Menu**

When using an Android device, to configure screen brightness use the following path:

**Swipe down from the very top of the screen > Display > Brightness > slide the brightness to the desired level**

Alternatively, tap the **Adaptive Brightness** toggle to allow the device to decide the optimal screen brightness based on the amount of ambient light.

**iOS Display & Brightness Menu**

When using an iOS device, to configure screen brightness, use the following path:

Swipe down from the top right corner and slide the brightness bar up or down to vary the brightness.

Alternatively, to configure brightness in the Settings menu, use the following path:
**Settings > Display & Brightness > slide the brightness to the desired level.**

# 1.3.3 GPS

Another common feature of mobile devices is the Global Positioning System (GPS). GPS is a navigation system that determines the time and geographical location of the device by using messages from satellites in space and a receiver on Earth. A GPS radio receiver uses at least four satellites to calculate its position based on the messages. GPS is very accurate, even used under most weather conditions. However, dense foliage, tunnels, and tall buildings can interrupt satellite signals. GPS receivers must have line-of-sight to GPS satellites and do not work indoors. Indoor Positioning Systems (IPS) can determine device location by triangulating its proximity to other radio signals, such as Wi-Fi access points.

GPS services allow app vendors and websites to know a device's location and offer location-specific services (such as local weather and advertising). This is called geotracking.

**Android Location Services**

To enable GPS on Android devices use the following path:

**Settings > Location > Tap on the toggle to turn location services on**

**iOS Location Services**

To enable GPS on iOS devices use the following path:

**Settings > Privacy & Security > Location Services > Turn location services on**

# 1.3.4 Lab - Mobile Device Features
# 1.3.5 Wi-Fi Calling
# 1.3.6 Mobile Payments
# 1.3.7 Virtual Private Network
# 1.3.8 Virtual Assistants

# 1.4 Passcode Locks
# 1.5 Cloud-Enabled Services for Mobile Devices
# 1.6 Mobile Device Software Security
# 1.7 Mobile Operating Systems and Security Summary


