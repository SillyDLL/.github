# SillyDLL Injector

> ⚠️ **EARLY TESTING PHASE** ⚠️
> 
> This project is currently in early testing. Many features are experimental and may not function as expected. Use at your own risk and please report any issues you encounter.

A lightweight, simple-to-use DLL injection utility for Windows applications.

## Overview

SillyDLL is a straightforward DLL injection tool designed for developers, testers, and software enthusiasts who need to modify application behavior at runtime. The injector supports both standard and manual mapping injection methods.

## Download

### Quick Start
1. Go to the [Releases](https://github.com/yourusername/SillyDLL/releases) page
2. Download the latest version
3. Extract the ZIP file to any location
4. Run SillyDLL.exe as administrator

### For Developers
Clone the repository:
```
git clone https://github.com/yourusername/SillyDLL.git
```

## Features

- **Multiple Injection Methods**: Support for LoadLibrary, Manual Mapping, and Thread Hijacking
- **Process Detection**: Automatic detection of running processes
- **Delay Injection**: Set timer for delayed injection
- **Signature Bypass**: Advanced techniques to avoid common anti-injection measures
- **Portable**: No installation required, runs from any directory
- **Minimal UI**: Clean, straightforward interface focused on functionality

## Usage

1. Launch SillyDLL
2. Select a target process from the dropdown or enter the process name/ID manually
3. Choose a DLL file to inject
4. Select your preferred injection method
5. Click "Inject" and monitor the status in the log window

## Command Line Usage

```
SillyDLL.exe --process [process_name] --dll [path_to_dll] --method [injection_method]

Options:
  --process, -p     Target process name or PID
  --dll, -d         Path to DLL file
  --method, -m      Injection method (1=LoadLibrary, 2=ManualMap, 3=ThreadHijack)
  --delay, -t       Delay in seconds before injection
  --hidden, -h      Run with no UI (silent mode)
```

## Known Issues
- Manual mapping may fail with certain protected processes
- Thread hijacking is not fully implemented in this test version
- Some antivirus software may flag the application

## Requirements

- Windows 7/8/10/11
- .NET Framework 4.6 or higher
- Administrator privileges (for some injection methods)

## Disclaimer

This tool is provided for educational purposes and legitimate software development scenarios only. Users are responsible for complying with all applicable laws and software licenses. SillyDLL should not be used to modify proprietary software without proper authorization.

## License

MIT License - See LICENSE file for details

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
