# FAQ

## Can't install the IDE on Win10

Windows may not recognize the IDE and there might be some problems when you install it. Windows Defender will pop up with a warning message.

![](.gitbook/assets/windows-protected-your-pc-2.png)

First, click on the "**More info"**.

Then more info will appear. Click "**Run anyway**".

## Can't open IDE on Mac

When you want to open the IDE, a new window appears:

![](.gitbook/assets/xnip2020-07-24_15-02-58.jpg)

👇 Here comes the solution:

* click **OK**.
* select ![](https://help.apple.com/assets/5EF110D6680CE23B38350954/5EF110E3680CE23B3835095C/en_GB/e043ddf1a45711e13f0b30612db65e21.png) &gt; **System Preferences**
* open the **Security & Privacy** Preferences pane
* select the **General** tab

![](.gitbook/assets/xnip2020-07-24_15-05-19.jpg)

* click the 🔒 icon
* enter your **Password**
* click **Unlock**

![](.gitbook/assets/xnip2020-07-24_15-05-35.jpg)

* click **Open Anyway**

![](.gitbook/assets/xnip2020-07-24_15-06-09.jpg)

* click **Open**

![](.gitbook/assets/xnip2020-07-24_15-06-19.jpg)

Now the IDE can run normally.

![](.gitbook/assets/xnip2020-07-24_15-07-20.jpg)

## Can't create new project on Windows

**Reason:** The IDE need to copy `MadMachine\Examples` and `MadMachine\Library` to your `Documents` directory when running for the first time.

**Solve:** Please make sure run the IDE as **Administrator** for the first time!

## IDE can't find the USB drive

This is due to the security feature of macOS. 

The latest versions of macOS introduce new security control. There are more requirements for application security. 

While our board needs to manage the files on the USB driver. So you need to enable **Full Disk Access** for IDE.

* select **System Preferences** in ![](https://help.apple.com/assets/5EF110D6680CE23B38350954/5EF110E3680CE23B3835095C/en_GB/e043ddf1a45711e13f0b30612db65e21.png)Apple menu
* open the **Security & Privacy** Preferences pane
* select the **Privacy** tab
* click **Full Disk Access** in the left column

![](.gitbook/assets/xnip2020-07-21_17-36-32.jpg)

* click the 🔒 icon
* enter your **Password**
* click **Unlock**

![](.gitbook/assets/xnip2020-07-21_17-39-35.jpg)

* click the icon **+**

![](.gitbook/assets/xnip2020-07-21_17-44-20.jpg)

* click **Application**
* find the **MadMachine**
* click **Open**

![](.gitbook/assets/xnip2020-07-21_17-46-34.jpg)

* click **Quit Now**

![](.gitbook/assets/xnip2020-07-21_17-49-14.jpg)

Now you can try to download your project again.

## **SwiftIO board reset repeatedly**

There is a maximum current limit for the USB port of your devices.

While some modules which is connected to the board may require a larger one.

Thus the board reset over and over again.

You can try these ways:

1 ****connect the board to USB port that can output larger power.‌

2 connect both download port and serial port on the board to USB ports

3 use a power bank to supply the board

## **USB driver can't be mounted**

Bad quality microUSB cable or third-party USB hub may cause this problem.

Just change it to a better one, and try again.

