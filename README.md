Windows Registry Editor Version 5.00
 
[-HKEY_CLASSES_ROOT\*\shell\runas]
 
[HKEY_CLASSES_ROOT\*\shell\runas]
@="獲取超級管理員權限"
"Icon"="C:\\Windows\\System32\\imageres.dll,-78"
"NoWorkingDirectory"=""
 
[HKEY_CLASSES_ROOT\*\shell\runas\command]
@="cmd.exe /c takeown /f \"%1\" && icacls \"%1\" /grant administrators:F"
"IsolatedCommand"="cmd.exe /c takeown /f \"%1\" && icacls \"%1\" /grant administrators:F"
 
[-HKEY_CLASSES_ROOT\Directory\shell\runas]
 
[HKEY_CLASSES_ROOT\Directory\shell\runas]
@="獲取超級管理員權限"
"Icon"="C:\\Windows\\System32\\imageres.dll,-78"
"NoWorkingDirectory"=""
 
[HKEY_CLASSES_ROOT\Directory\shell\runas\command]
@="cmd.exe /c takeown /f \"%1\" /r /d y && icacls \"%1\" /grant administrators:F /t"
"IsolatedCommand"="cmd.exe /c takeown /f \"%1\" /r /d y && icacls \"%1\" /grant administrators:F /t"
 
[-HKEY_CLASSES_ROOT\dllfile\shell]
 
[HKEY_CLASSES_ROOT\dllfile\shell\runas]
@="獲取超級管理員權限"
"HasLUAShield"=""
"NoWorkingDirectory"=""
