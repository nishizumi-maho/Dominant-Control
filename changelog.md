# Changelog

All notable changes to Dominant Control for iRacing will be documented in this file.

---

## [1.0.0] - 2024-12-11

### 🎉 Initial Release

First public release of the iRacing Control Interface accessibility tool.

### Core Features

#### Accessibility Support
- **Simplified Control Access**: Map vehicle adjustments to accessible keyboard keys or controller buttons
- **Keyboard-Only Mode**: Full functionality without joystick/controller for maximum compatibility
- **Device Management**: Selectively enable/disable input devices
- **Visual Feedback**: Real-time HUD overlay showing current control values
- **Preset System**: Quick access to common values with single button press
- **Standalone Executable**: No Python installation required, just download and run
- **Auto Car/Track Detection**: Automatically detects current car and track from iRacing
- **Per-Car Configuration**: Save separate configurations for each car
- **Per-Track Presets**: Load different setups for different tracks automatically
- **Multi-Variable Combo Macros**: Adjust multiple controls with a single button press
- **Customizable HUD Overlay**: Draggable, real-time telemetry display with full customization
- **Multiple Timing Profiles**: Aggressive, Casual, Relaxed, and Custom timing options

#### Accessibility Features
- **Simplified Control Access**: Map any vehicle adjustment to accessible inputs
- **Keyboard-Only Mode**: Full functionality without joystick/controller
- **Device Management**: Selectively enable/disable input devices
- **Visual Feedback**: Real-time display of all control values
- **Preset System**: Quick access to common values without multiple presses

#### Educational Components
- **Telemetry Visualization**: Real-time monitoring of vehicle parameters
- **Configuration Management**: Learn about setup management
- **Data Analysis Tools**: Study how adjustments affect vehicle behavior

#### User Interface
- **CONFIG/RUNNING Mode Toggle**: Clear separation between configuration and active use
- **Tabbed Interface**: Organized control management
- **Scan Function**: Automatic detection of available driver controls
- **Per-Car HUD Configuration**: Customize display for each vehicle
- **Overlay Styling**: Custom colors, fonts, opacity settings

### Documentation
- Complete user guides and setup instructions
- Quick start guide for 5-minute setup
- Comprehensive FAQ
- Legal documentation and terms of use
- Troubleshooting guides

### Known Limitations
- **Force Feedback Compatibility**: Application must be started before iRacing to maintain force feedback
  - **Workaround**: Start app first, then iRacing
  - **Alternative**: Use Keyboard-Only Mode (eliminates issue completely)
  - **Technical cause**: Python joystick library limitation on Windows
- See INSTALLATION.md for detailed startup order instructions

### Security & Privacy
- **Complete README**: Comprehensive feature overview and usage guide
- **Quick Start Guide**: Get running in 5 minutes
- **Installation Guide**: Detailed setup instructions with troubleshooting
- **Legal Documentation**: Clear disclaimers, license, and terms of use
- **User Agreement**: Responsible use guidelines

### Security & Privacy
- **No External Connections**: Application works entirely offline
- **Local Storage Only**: All configurations stored locally
- **No Telemetry**: No tracking, analytics, or data collection
- **No Internet Required**: Except for iRacing itself

### Compliance & Ethics
- **Accessibility Focus**: Designed for users with genuine needs
- **Educational Purpose**: Learning tool for telemetry and vehicle dynamics
- **Clear Documentation**: Comprehensive legal and ethical guidelines
- **Responsible Use Framework**: Guidelines for appropriate usage

---

## Version Numbering

This project uses [Semantic Versioning](https://semver.org/):
- **MAJOR**: Incompatible changes or major rewrites
- **MINOR**: New features, backwards compatible
- **PATCH**: Bug fixes, backwards compatible

---

## Planned Future Improvements

### Under Consideration
- Additional timing profile options
- Enhanced HUD customization
- More telemetry data points
- Configuration import/export
- Backup and restore functions

**Note**: Future updates depend on user feedback and community needs. No timeline promised.

---

## Support Policy

- **Current Version (3.x)**: Active support
- **Previous Versions**: No longer supported
- **Updates**: Released as needed, manual download from Releases

---

## Reporting Issues

Due to the sensitive nature of this software:
- Do NOT post issues publicly
- Contact privately through authorized channels
- Include version number and detailed description
- Provide steps to reproduce
- Include relevant error messages

---

## Distribution Notes

### Release Format
- **Standalone Executable**: Windows x64 .exe file
- **Documentation**: Complete set of markdown files
- **Package**: Distributed as ZIP archive

### Supported Platforms
- Windows 10 (64-bit) - Build 1809 or later
- Windows 11 (all versions)

### File Structure
```
DominantControl_v1.0.0.zip
├── DominantControl.exe
├── README.md
├── QUICKSTART.md
├── INSTALLATION.md
├── DISCLAIMER.md
├── LICENSE.md
├── FAQ.md
├── CHANGELOG.md (this file)
├── TECHNICAL.md
└── _READ_ME_FIRST.txt
```

---

## First-Time Setup

This is the initial release. For setup instructions:
1. See QUICKSTART.md for fast 5-minute setup
2. See INSTALLATION.md for detailed instructions
3. **Remember**: Start the app BEFORE starting iRacing to preserve force feedback
4. Or use Keyboard-Only Mode to avoid the issue entirely

---

## Acknowledgments

### Built With
- Python 3.9
- iRacing SDK
- tkinter (GUI framework)
- pygame (input handling)
- keyboard (key capture)
- pyttsx3 (text-to-speech)

### Principles
- Accessibility first
- Educational value
- Ethical use
- Community responsibility

---

## Legal

This software is proprietary and closed-source. See LICENSE.md for complete terms.

**Not affiliated with iRacing.com Motorsport Simulations, LLC.**

---

## Version Archive

### [1.0.0] - 2024-12-11
Initial release - First production version

---

**For latest version, check the Releases section.**

*Keep your version updated for best stability and features.*
