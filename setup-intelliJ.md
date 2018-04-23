# IntelliJ Full Setup

## Pre-requisites :
### IntelliJ Ultimate : 

- Download (Ultimate Version, JEE not available in community edition) : https://www.jetbrains.com/idea/download/download-thanks.html?platform=windows
- After setup downloaded, launch the .exe and install IntelliJ
- At the end, an activation window will pop up, connect to the app with your JetBrains account or enter your serial key for IntelliJ (available through your JetBrains account on jetbrain's website).

### Java

- Download and install JavaSE 8 : http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html (tested with ver. 8u171)

### GlassFish

- Download GlassFish 4.1.2 : http://download.java.net/glassfish/4.1.2/release/glassfish-4.1.2.zip
- Extract zip at a known location (example : C:/Packages/GlassFish4.1.2), path will be required during IntelliJ's project setup.

### Android Studio

- Download : https://dl.google.com/dl/android/studio/install/3.1.1.0/android-studio-ide-173.4697961-windows.exe
- Install Android Studio (let all choices by default)
- When the installation is done, launch Android Studio and clic the Configure dropdown, then SDK Manager, a new window will be opened.
![SDK Manager](https://cdn.pbrd.co/images/HhWkwyd.png)

- On the new window, you can see all the Android SDK versions installed and the default location for your installed SDKs. **Please note your Android SDK folder location, it will be used to configure IntelliJ later.**

![Android SDK Versions](https://cdn.pbrd.co/images/HhWo5oN.png)
- In order to install a SDK version, check it, then clic Apply.

 ## IntelliJ Setup

### JDK & Android SDK Setup

- Open IntelliJ (if it automatically starts by loading your project, clic **Cancel** while your project is being loaded by IntelliJ to access to the Welcome Screen)
- On the Welcome Screen, clic Configure -> Project Defaults -> Project Structure, a new window will pop up.

![Welcome Screen](https://cdn.pbrd.co/images/HhW9x7b.png)

- In the new window, select SDKs on the left, then clic the green plus sign on top, and clic JDK

![Add JDK Reference](https://cdn.pbrd.co/images/HhWhH2l.png)
- And locate your JDK install folder (default = C:\Program Files\Java\jdk1.8.0_171) and clic OK.

- Do the same for Android SDK (default path = C:\Users\Username\AppData\Local\Android\Sdk)

![Add Android SDK reference](https://cdn.pbrd.co/images/HhWj4aS.png)
- Finally clic Apply and OK.

### GlassFish Setup

- Again on the IntelliJ Welcome Screen, clic Configure -> Settings

![Setup GlassFish](https://cdn.pbrd.co/images/HhWzhWQ.png)

- Select **Build, Execution, Deployment** in the left column then **Application Servers**
- Clic on the **"+"** sign and select GlassFish Server
- Enter the path of your GlassFish install folder in **GlassFish Home** field.
- Clic **OK**, **Apply** and **OK**

![GlassFish Configuration](https://cdn.pbrd.co/images/HhWCCcU.png)

## New Project

 - Open IntelliJ and Create a new project.
	- Select **Java Enterprise** on the left column.
	- **Project SDK** : Select **1.8** from the dropdown
	- **JavaEE version** : **Java EE 8**
	- **Additional Libraries & Frameworks** : check **Web Application** and **Struts2**
	- **Application Server** : Select **GlassFish** from the dropdown.

- You should have a similar window :
![New Project Configuration](https://cdn.pbrd.co/images/HhWt9Et.png)

- Clic **Next**, then name your project and clic **Finish**.