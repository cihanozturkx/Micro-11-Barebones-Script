Statement from developer:
> I was publishing the customized version of Windows on different forums and communities since 2011, but as I got older, I thought of sharing my knowledge with everyone through this Powershell Script.

This PowerShell script was written by "mackyreddy", the maker of Windows Micro 11 Barebone ISOs, and is shared here with his consent. All credits goes to him. I will not change the code, but only publish new version if developer shares it. So feel free to fork and contribute!

## Features
- **Basically everything is removed beside basic desktop functionality**
- Deep component (CBS aware) removal
- WinSxS clean-up
- Registry clean-up
- Registry tweaks
- Supports both x64 and ARM64 ISOs
- Tested on Windows 11 Home 26H2 build 26300.9550. **The ISO file is 1.07 GB and the total installation size came around 3.80 GB**

## Requirements
- Stock Windows 11
- PowerShell 7.7

## Notes
- No GUI or selections, everything is done by PowerShell. (For now)
- WinRE, Windows Defender, Windows Updates are removed. No support for updates or servicing.
- You can try running script on debloated Windows. But you will face DISM errors since DISM relies on WinSxS. A stock Windows is recommended.
- If you do not want ESD compression, you can replace "compress:recovery" values ​​in the script with "compress:max" or "compress:fast"

## Workflow
<details>
  <summary>Click to expand</summary>

- Folder Ownership Acquisition
- System Package Removal
- Aggressive Manual File Cleanup
- WinSxS Reduction
- Registry Tweaks and Configuration
- Windows Services Optimization
- Custom File and Application Injection
- Install.wim Registry Cleanup
- Boot.wim Manual File Cleanup
- Boot.wim Registry Cleanup
- WIM-to-ESD Conversion
- ISO Directory Cleanup
- ISO Creation
- Temporary File Cleanup
- Done
</details>


<p align="center">
  <img src="https://www.elevenforum.com/attachments/micro-11-barebones-processes-detailed-view-webp.186140/" width="49%">
  <img src="https://www.elevenforum.com/attachments/micro-11-barebones-memory-usage-webp.186138/" width="49%">
</p>
