# win11-oled-black-titlebar

![Comparison](https://github.com/QinnShou/win11-oled-black-titlebar/blob/main/github%20demo%20title.jpg) 

(I have no idea why the icon vanished)

A registry tweak for Windows 11 that makes title bars pure black, helping to reduce OLED screen burn-in, especially for fullscreen programs and apps. A gray variant is also included for aesthetic preferences.

## Files Included
- **`win11_blacktitle.reg`**: Applies pure black title bars (#000000, #000000). This one is OLED-friendly.
- **`win11_graytitle.reg`**: Applies gray title bars (#404040, #101010).
- Content:

```reg
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\Microsoft\Windows\DWM]
"AccentColor"=dword:ff000000
"AccentColorInactive"=dword:ff000000
"ColorPrevalence"=dword:1
"ColorizationColor"=dword:ff000000
```


## Usage
0. Take note of your original register value here: HKEY_CURRENT_USER\Software\Microsoft\Windows\DWM
   "AccentColor", "AccentColorInactive", "ColorPrevalence", "ColorizationColor"
1. Download the `.reg` file of your choice from the repository.
2. Double-click the file to apply the changes to your registry.
3. Restart your PC to see the changes.

## Important Notes
- Modifying the registry can have unintended effects. Use these files at your own risk.
- Always back up your registry before applying any changes.
