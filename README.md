![GitHub release (latest by date)](https://img.shields.io/github/v/release/infinitepower18/wsa-sideloader)
![MS Store downloads](https://img.shields.io/badge/ms%20store%20downloads-15k%2B-brightgreen)
![GitHub all releases](https://img.shields.io/github/downloads/infinitepower18/WSA-Sideloader/total?label=github%20downloads)
![Uses Python 3.10](https://img.shields.io/badge/python-3.10-yellow)
![GitHub](https://img.shields.io/github/license/infinitepower18/wsa-sideloader)

# WSA Sideloader
WSA Sideloader is a tool that is used to easily install APK files on Windows Subsystem for Android. The program has been designed with simplicity and ease of use in mind.

![image](https://user-images.githubusercontent.com/44692189/172241903-a66b7d9f-0692-4178-81e4-561e3978ed9b.png)

## Download

<p><a href="https://www.microsoft.com/store/apps/9NMFSJB25QJR?cid=ghreadme">
<img src="https://getbadgecdn.azureedge.net/images/English_L.png" width="216" height="78">
</a></p>

You can also download from [GitHub Releases](https://github.com/infinitepower18/WSA-Sideloader/releases) or via winget using the command `winget install wsa-sideloader`
                
## Getting started

Make sure you have Windows Subsystem for Android installed on your Windows 11 machine. If you don't already have it, download it from [here](https://aka.ms/AmazonAppstore). You don't need to use the Amazon Appstore, however don't uninstall it as it will remove the subsystem.

If you're outside the US, change your PC region setting to United States, you should then be able to download Amazon Appstore which contains the subsystem. You can change it back once you have installed it.

![image](https://user-images.githubusercontent.com/44692189/173249543-1a96679f-0773-4e41-8ddc-10e71ae189c2.png)

Amazon Appstore for WSA is currently not available outside the US and Japan, but Microsoft plans to make the appstore and WSA available in France, Germany, UK, and Italy by the end of this year.

Enable developer mode in WSA settings. It is also recommended you enable continuous mode, however WSA Sideloader will attempt to start the subsystem for you if it's not running.

![image](https://user-images.githubusercontent.com/44692189/182655019-5cd310c6-8bbd-43b6-a60b-ebd35c12748c.png)

Choose the APK file you want to install and click the Install button. In most cases, you do not need to change the ADB address. You can also install an APK file right from File Explorer, web browsers and other supported programs.

## Known issues

### No new ARM64 builds
No new builds will be released until further notice. More details can be found [here](https://github.com/infinitepower18/WSA-Sideloader/discussions/30).

An ARM64 version of [version 1.1.10](https://github.com/infinitepower18/WSA-Sideloader/releases/tag/v1.1.10) is available if you really want to use a native version. However please be aware that features like Explorer integration are not available in this version.

## FAQ

### I installed the app successfully, but the app crashes while using it or doesn't work as intended.
WSA Sideloader is just an APK installer. Whether the app actually works or not depends on the app and the subsystem. Please be aware that apps that require Google Play Services may not work properly on WSA. You may try solutions such as [Magisk on WSA](https://github.com/LSPosed/MagiskOnWSALocal) if you want Google Play functionality.

You may check [this page](https://github.com/riverar/wsa-app-compatibility) for a list of compatible apps.

### Why does it take so long for new updates to be released on Microsoft Store?
As much as I want the updates released on GitHub and Microsoft Store at the same time, this is something beyond my control. Sometimes they take up to 24 hours to approve the update, sometimes few days. There's nothing I can do about it unfortunately.

### I would like to see [feature name] in your program. When can you implement it?
I am open to suggestions and will try my best to add more relevant features to the program over time. If you have any suggestions you can open an issue with your suggestion. I usually fix bugs and maintain stability of the program before adding more stuff to it so it may take some time.

### Where can I see a list of installed WSA apps?
You can press the "Installed apps" button to bring up a list of apps installed on the WSA. You can launch and uninstall apps through it as well as manage notifications, permissions etc. for each app. WSA apps are also present on the start menu and you can right click to uninstall just like any other Windows program.

If you would like to launch a list of installed apps right from the start menu, I have made an app for that. You can download it [here](https://github.com/infinitepower18/WSA-InstalledApps).

### What's the best place to download APK files?
My personal recommendaton is [APKMirror](https://www.apkmirror.com/), it is run by Android Police founder Artem Russakovskii.

## Support

Need help using WSA Sideloader? Post in the project's [discussions tab](https://github.com/infinitepower18/WSA-Sideloader/discussions). Found a bug or want to make a feature request? Visit the [issues page](https://github.com/infinitepower18/WSA-Sideloader/issues).

## Privacy Policy

Please [click here](https://ahnafmahmud.me/apps/WSA-Sideloader/PrivacyPolicy.html) to view the privacy policy.

TLDR - No information is collected by this application.

## Contributing

Whether it's a bug fix or a new feature, contributions to the project are always welcome! To get started, make sure you have [Python 3.10](https://www.python.org/downloads/windows/) and [Git](https://gitforwindows.org/) installed. Then clone this repo and install the required packages using `pip install -r requirements.txt`.

Please test the program before making your pull request. Starting from version 1.3.0, WSA Sideloader is compiled into an executable file using Nuitka.

To compile from source, follow the below instructions:

1. Download the latest version of [Python 3.10 64 bit](https://www.python.org/downloads/windows/)
2. Install Nuitka via pip using the command `pip install nuitka`
3. Clone the repository, and install the required dependencies using the command `pip install -r requirements.txt` in the root directory.
4. In the root directory run the command `nuitka --standalone sideloader.py --enable-plugin=tk-inter --windows-disable-console`. This may take some time depending on your computer.
5. Copy the icon.ico file and adbfiles folder to the sideloader.dist folder.

As this program is a APK installer for Windows Subsystem for Android, please make sure you are running Windows 11 with WSA installed.

## Disclaimer
This project is not affiliated with Microsoft or Google in any way.
