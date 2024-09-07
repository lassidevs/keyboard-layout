# MSKLC build script (US-international, No dead keys)

This repo contains a klc build script for Microsoft Keyboard Layout Creator. 

I have a need for Finnish characters in my job and day-to-day life. This proves difficult as I'm running a US keyboard for programming, which doesn't include characters like ä and ö. Normally a fix would be to use English (United States) international layout, but this comes with dead keys that messes up writing flow and adds unwanted features. This script initiates a normal US international layout with support for non-ASCII characters (such as ä and ö), but removes dead keys completely. 

## How to use
1. Install MSKLC from https://www.microsoft.com/en-us/download/details.aspx?id=102134
2. Download the source file from this repo (us_international_no_dead_keys.klc)
3. Open MSKLC and load the aforementioned source file. Then click Project > Build DLL and setup package > complete the setup.
- The build process can take a few minutes. After the build completes, it'll add several installer files to your home directory, for me it was "C:\Users\{username}\Documents\usintgr"
4. Run The installer
- Depending on your computer's architecture, you'll run the appropriate installer shown below. To check you architecture, open cmd and run command "wmic os get osarchitecture" <br /><br />
-Run the _amd64 suffixed installer if you're running a 64-bit version of Windows running on a standard x64 (AMD or Intel) processor. This is likely what you'll be running. <br />
-Run the _i386 suffixed installer if you're running a 32-bit version of windows. <br />
-Run the _ia64 suffixed installer if you're running an intel Itanium microprocessor. This chip was dicontinued ages ago and is highly unlikely you have it. <br />

5. Restart PC
- Since the installer makes registry changes, you'll need to restart your pc for the changes to propagate and see your newly installed keyboard.
6. Profit
- If you did everything correctly, your new keyboard should be available for selection.
To add the keyboard (windows 11), go to settings > time & language > Language & region > English (United States) > Language options > Add a keyboard.
