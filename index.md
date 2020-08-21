title:Hello!
## Welcome to the MyTech Specialist script repository 

These codes can be ran by copying and pasting them into Notepad, and then saving as a .bat file.

```markdown

Title = MyTech Specialist Win10 Cleaner

@echo off
echo Deleting temp files...
	del "%tmp%\*.*" /s /q /f
	FOR /d %%p IN ("%tmp%\*.*") DO rmdir "%%p" /s /q
echo Temp files deleted
echo Deleting cookies...

ping localhost -n 3 >nul

del /f /q "%userprofile%\Cookies\*.*"
echo Cookies deleted
echo Starting disk cleanup
c:\windows\system32\cleanmgr.exe /dc /sageset: 1
c:
cd \
cd c:\windows\prefetch
del *.* /q
echo Disk cleanup started
pause

```
