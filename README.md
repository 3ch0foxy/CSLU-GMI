# CSLU-GMI | Memory Analysis Workshop Materials
**Repository**: https://github.com/3ch0foxy/CSLU-GMI

Hello everyone! This repository contains :

## Required Tools

1. **MemProcFS** - Memory process file system for advanced memory analysis  
   Download: [https://github.com/ufrisk/MemProcFS](https://github.com/ufrisk/MemProcFS)

2. **FLARE VM** - Windows security analysis environment  
   Installation Guide: [Affan's FLARE-VM Setup Guide](https://github.com/plnsgr/CSLU_Malware-Analysis_Workshop)

3. **WinPmem** - Memory acquisition tool  
   Download: [https://github.com/Velocidex/WinPmem/releases](https://github.com/Velocidex/WinPmem/releases)  
   - Select the appropriate `winpmem.exe` version for your Windows system
   - Use the most recent release version

4. **7-Zip** - File archiver utility  
   Download: [https://7-zip.org/](https://7-zip.org/)

## Workshop Setup Instructions

1. Install FLARE-VM
2. Download all required tools to your analysis machine
3. Place WinPmem executable in your FLARE-VM environment
4. Verify all tools are accessible from your system PATH

> **Note**: Ensure your analysis machine meets these requirements:  
> - Windows 10/11 (64-bit)  
> - 8GB+ RAM (16GB recommended)  
> - 50GB+ free disk space (For the challenges)

## Challenge Files Download

The challenge files are provided as split archives. To use them:

1. Install [GitHub CLI](https://cli.github.com/)
2. Run these commands:
```powershell
# Download all challenge files
gh release download -D ./challenges

# Reassemble and extract
cd challenges
7z x FINAL_challenges.7z.001
7z x compressed_challenges.7z
```
3. You'll now have these memory images:
   - `exfil.raw`
   - `persistence.raw`
   - `rogue.raw`

> Note: Total extracted size is 26GB. Ensure you have sufficient disk space.
