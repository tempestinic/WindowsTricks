# WindowsTricks
A compilation of registry tricks.

## Restore previous Context Menu (Right Click Menu) in Windows 11
If you don't like the new Windows 11 context menu you can restore the old one using this method:
Use the file "Restore Windows 11 context menu.reg" or manually add the following registry keys

```ini
[HKEY_CURRENT_USER\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}]

[HKEY_CURRENT_USER\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32]
@=""
```

## Disable CTRL+ALT+DEL on login (Windows server)
Use the file "DisableCtrlAltDel.reg" or manually add the following registry keys to disable the request of CTRL+ALT+DEL to access the login screen

```ini
[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon]
"DisableCAD"=dword:00000001

[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System]
"disablecad"=dword:00000001
```

## Open Classic Notification Area Icons
Press Win+R to open the Run prompt on your computer. Then, enter this command:

explorer shell:::{05d7b0f4-2121-4eff-bf6b-ed3f69b894d9}
