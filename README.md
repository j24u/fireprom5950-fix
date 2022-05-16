# AMD Firepro M5950 BUG fix (Windows + Linux)

WINDOWS FIX

I had an HP EliteBook Workstation 8570W equipped with the IN-Board graphic card AMD FirePro M5950. The chip had a bug currently don't know if it was only mine the one with it, anyway every time the chipset would set to PERFORMANCE mode and the power would not get used (ex, gaming) the desktop interface would start bugging out showing blue and black lines making the laptop unable to use. 
I discovered that changing the settings in the FirePro Panel under the Power section to battery saver would get the laptop saved from all the screen flickering and glitching. Change the settings even if your laptop would change its power mode while on AC power. This is the saving for the Windows OS, doesn't matter the version, works even in WIN 11.

![Untitled](https://user-images.githubusercontent.com/90705698/168669546-48e28121-c892-4ee5-85ce-94d41d495828.png)

--------------------------------------------------------------------------------------------------------------------------------------------------------
LINUX FIX

In linux you have to download the TLP package.

$ sudo apt install tlp

After installing the package, you can easily replace the tlp.conf in this repository with the one you have by default in your system and it can be found in
/etc/tlp.conf. After replacing the tlp you can launch the program anytime you start your laptop with the command.

$ sudo tlp start


This is it, guys. I hope it comes to help to all of you.
