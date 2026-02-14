# Nux Programming Language - Windows Distribution

```
████     ██████████████      ███╗    ██╗██╗    ██╗██╗    ██╗
████     ██████████████      ████╗   ██║██║    ██║╚██╗  ██╔╝
████     ████                ██╔██╗  ██║██║    ██║ ╚██╗██╔╝ 
████     ████                ██║╚██╗ ██║██║    ██║  ╚███╔╝  
██████████████████████       ██║ ╚██╗██║██║    ██║   ███║   
██████████████████████       ██║  ╚████║██║    ██║  ██╔██╗  
         ████     ████       ██║   ╚███║██║    ██║ ██╔╝╚██╗ 
         ████     ████       ██║    ╚██║██║    ██║██╔╝  ╚██╗
█████████████     ████       ██║     ╚█║╚██████╔╝██║      ██║
█████████████     ████       ╚═╝      ╚╝ ╚═════╝ ╚═╝      ╚═╝
```

**Version:** 1.0.0  
**Platform:** Windows 10/11 (x64)

## Quick Start

Install Nux by running the installer as Administrator:

```cmd
setup.bat
```

## System Requirements

- **OS:** Windows 10 (build 10586+) or Windows 11
- **Architecture:** x64 (64-bit)
- **Disk Space:** ~100 MB
- **RAM:** 512 MB minimum

## Installation

### 1. Extract the Package

Extract the ZIP file to a folder, e.g., `C:\nux_pack_windows`

### 2. Run the Installer as Administrator

**Right-click** `setup.bat` and select **"Run as administrator"**

The installer will:
- ✓ Check administrator privileges
- ✓ Create installation directories
- ✓ Install Nux runtime and libraries
- ✓ Add Nux to system PATH
- ✓ Register .nux file extension

### 3. Verify Installation

Open a **new** Command Prompt or PowerShell and run:

```cmd
nux --version
```

You should see: `Nux v1.0.0 (Windows)`

## Getting Started

### Start the REPL

```cmd
nux repl
```

### Run Example Programs

```cmd
REM Hello World
nux examples\hello.nux

REM Web Server
nux examples\web_server.nux

REM AI Demo
nux examples\ai_demo.nux
```

### Create Your First Program

```cmd
echo import "std.io"; println("Hello, Nux!"); > hello.nux
nux hello.nux
```

## What's Included\r

- **Standard Libraries** (79 files)
  - `lib\std\` - Core utilities, I/O, networking, graphics
  - `lib\ai\` - Neural networks, transformers, GANs, RL
  - `lib\os\` - Kernel, scheduler, memory management
  - `lib\embedded\` - Hardware control, GPIO, sensors

- **Examples**
  - `hello.nux` - Basic syntax and I/O
  - `web_server.nux` - HTTP server
  - `ai_demo.nux` - Neural network training

- **Tools**
  - `nux.bat` - Runtime and REPL
  - `nuxc.bat` - Compiler
  - `nuxr.bat` - Script runner

## Windows-Specific Features

- **File Association:** Double-click .nux files to run them
- **ANSI Colors:** Full color support in Windows Terminal
- **PowerShell Integration:** Works in both CMD and PowerShell
- **Registry Integration:** Proper file type registration

## Troubleshooting

### Access Denied

Make sure to run `setup.bat` as Administrator:
1. Right-click `setup.bat`
2. Select "Run as administrator"

### Command Not Found

Restart your terminal (Command Prompt or PowerShell) after installation.

If the issue persists, manually add to PATH:
1. Open System Properties → Advanced → Environment Variables
2. Add `C:\Program Files\Nux\bin` to PATH

### ANSI Colors Not Working

Use Windows Terminal (recommended) or update Windows to build 10586+.

### Antivirus Blocking Installation

Some antivirus software may flag the installer. Add an exception for:
- `C:\Program Files\Nux\`
- `setup.bat`

## Uninstallation

Run the installer with the uninstall flag:

```cmd
setup.bat uninstall
```

Or manually:
1. Delete `C:\Program Files\Nux`
2. Remove from PATH in Environment Variables
3. Delete registry keys under `HKCU\Software\Classes\.nux`

## Documentation

- **Language Guide:** https://nux-lang.org/docs
- **API Reference:** https://nux-lang.org/api
- **Examples:** https://github.com/nux-lang/examples

## Support

- **Issues:** https://github.com/nux-lang/nux/issues
- **Community:** https://discord.gg/nux-lang
- **Email:** support@nux-lang.org

## License

Nux Programming Language is released under the MIT License.  
See LICENSE.txt file for details.

---

**Happy Coding!** 🚀
