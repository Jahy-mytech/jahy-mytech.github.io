
## Welcome to the MyTech Specialist script repository 

If you have any issues you can contact me on Discord: Jahy#1948

These codes can be ran by copying and pasting them into Notepad, and then saving as a .bat file.
The purpose of these codes are to easily delivery on the more frequently asked questions in the MyTech discord, such as checking RAM speed, freeing up space in Windows, checking hardware, etc. If you have any suggestions feel free to let me know. Thanks.

#RAM Check Tool
```
title = RAM Check
wmic memorychip get devicelocator, speed, manufacturer, status, serialnumber
```

#Windows 10 Quick Clean
```
Title = MyTech Specialist Quick Clean
@echo off
	del "%tmp%\*.*" /s /q /f
	FOR /d %%p IN ("%tmp%\*.*") DO rmdir "%%p" /s /q
ping localhost -n 3 >nul
del /f /q "%userprofile%\Cookies\*.*"
c:\windows\system32\cleanmgr.exe /dc /sageset: 1
c:
cd \
cd c:\windows\prefetch
del *.* /q
pause
```
