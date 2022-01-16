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
