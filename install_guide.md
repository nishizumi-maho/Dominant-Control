# Installation Guide

Simple setup instructions for the iRacing Control Interface.

## ⚠️ Before Installing

**Please Read:**
- This software is for accessibility assistance and educational purposes only
- Intended for drivers with physical limitations or equipment constraints
- Should be used in private testing sessions
- Users are responsible for compliant usage with all platform terms of service
- Not intended for competitive racing environments

By installing this software, you acknowledge these terms and agree to use it responsibly.

---

## System Requirements

### Minimum Requirements
- **Operating System**: Windows 10 (64-bit) or Windows 11
- **RAM**: 4 GB
- **Disk Space**: 100 MB
- **iRacing**: Valid subscription and installation

### Recommended Specifications
- **Operating System**: Windows 11
- **RAM**: 8 GB or more
- **Monitor**: 1920x1080 or higher (for HUD overlay)
- **Input Devices**: Keyboard and/or game controller

---

## Installation (Simple - No Python Required!)

### Step 1: Download

1. Go to the **Releases** section
2. Download the latest `iRacingControlManager_v1.0.0.zip` file
3. Save to a location you can remember (e.g., Downloads folder)

### Step 2: Extract Files

1. **Right-click** the downloaded ZIP file
2. Select **"Extract All..."**
3. Choose a destination (recommended: `C:\iRacingControl\`)
4. Click **"Extract"**

### Step 3: Run the Application

1. Navigate to the extracted folder
2. Double-click **`iRacingControlManager.exe`**
3. Application will start!

**That's it! No installation, no Python, no dependencies to worry about.**

---

## First-Time Setup

### Windows Security Warning

When first running, Windows may show a security warning:

```
Windows protected your PC
Microsoft Defender SmartScreen prevented an unrecognized app from starting
```

**This is normal** for applications without expensive code-signing certificates.

**To proceed:**
1. Click **"More info"**
2. Click **"Run anyway"**

The application is safe - this warning appears for many legitimate applications.

### Initial Launch

On first run, the application will:
1. Create configuration folder: `%APPDATA%\DominantControl\`
2. Initialize default settings
3. Open the main window

You're now ready to configure!

---

## Configuration Steps

### For Accessibility Users

If you have physical limitations or equipment constraints:

#### 1. Start iRacing
- Launch iRacing
- Enter a **PRIVATE practice session**
- Get into the car (Drive mode)

#### 2. Launch Application
- Run `iRacingControlManager.exe`
- Wait for it to connect to iRacing

#### 3. Enter CONFIG Mode
- Click the **"Mode: RUNNING"** button
- It will change to **"Mode: CONFIG"**

#### 4. Scan Controls
- Click **"🔍 SCAN DRIVER CONTROLS"**
- Application will detect available controls for your car

#### 5. Configure Keys
For each control you need to access:
- Click the **"Set Increase (+)"** button
- Press the key you want to use
- Click the **"Set Decrease (-)"** button
- Press the key you want to use

These should be keys that:
- You can easily reach
- Don't conflict with iRacing controls
- Are comfortable for your physical situation

#### 6. Set Up Presets (Optional but Recommended)
For quick access to specific values:
- Enter a target value (e.g., "52.5" for brake bias)
- Click **"Set Bind"**
- Press a keyboard key or controller button
- Repeat for common values you use

#### 7. Configure HUD (Optional)
- Go to **"HUD / Overlay"** tab
- Check which values you want to display
- Customize colors, font size, opacity
- Click **"Apply Style"**

#### 8. Save Configuration
- Click **"Save Current"**
- Enter car and track names
- Your settings are now saved for this car/track combination

#### 9. Switch to RUNNING Mode
- Click the mode button again
- Now in **"Mode: RUNNING"**
- Application is active

#### 10. Test in Private Session
- Test each control you configured
- Verify HUD displays correctly
- Adjust timings if needed (Options → Timing Adjustments)

---

## For Educational Use

If using for learning purposes:

1. **Launch in practice session** - Start iRacing private practice
2. **Run application** - Start the .exe file
3. **Scan controls** - See what's available
4. **Observe telemetry** - Watch real-time values in HUD
5. **Experiment** - Try different configurations
6. **Learn patterns** - Study how settings affect behavior

---

## Device Configuration

### Keyboard Only Mode

If you only want to use keyboard (no joystick/controllers):
1. Check **"Keyboard Only Mode"**
2. Application will restart
3. Only keyboard inputs will be available

### Managing Input Devices

If using controllers/joysticks:
1. Click **"🎮 Manage Devices"**
2. **Check** devices you want to use
3. **Uncheck** devices to ignore (recommended: uncheck wheel/pedals)
4. Click **"Save and Apply"**

**Tip**: Only enable button boxes or separate controllers, not your steering wheel device.

---

## File Locations

### Application Files
Located where you extracted:
```
C:\DominantControl\
├── DominantControl.exe
├── README.md
├── LICENSE.md
└── (other documentation files)
```

### Configuration Files
Automatically created in:
```
%APPDATA%\DominantControl\configs\
└── config_v3.json
```

**Your configurations are separate from the application files**, so updates won't delete your settings.

---

## Troubleshooting

### Application Won't Start

**"Missing DLL" or "VCRUNTIME" errors:**
- Install Microsoft Visual C++ Redistributable
- Download from Microsoft's website (free)
- Restart computer after installation

**"Windows protected your PC" won't go away:**
- Right-click the .exe → Properties
- Check "Unblock" at the bottom
- Click Apply → OK
- Try running again

**Application crashes immediately:**
- Run as Administrator (right-click → Run as administrator)
- Check Windows Event Viewer for error details
- Ensure Windows 10/11 64-bit

### Cannot Connect to iRacing

**"No connection" or "Cannot detect iRacing":**
- Ensure iRacing is running
- Must be in a session (not menus)
- Must be in the car (Drive mode)
- Try Alt+Tab to iRacing, then back to the app
- Restart both iRacing and the application

### Controls Not Working

**Buttons don't do anything:**
- Verify you're in **RUNNING mode** (not CONFIG)
- Check the mode button at the top
- Ensure keys are configured (should show key names, not "Set Increase")
- Test in a private practice session
- Check that the correct input device is enabled

**Adjustments are too slow/fast:**
- Go to Options → Timing Adjustments
- Try a different profile (Aggressive/Casual/Relaxed)
- Or use Custom to fine-tune

### HUD Not Showing

**Overlay not visible:**
- Click Options → Show/Hide Overlay
- Check if it's off-screen (try dragging)
- Verify variables are marked visible in "HUD / Overlay" tab
- Adjust opacity (might be too transparent)
- Try clicking in the application window first

**HUD shows "--" for all values:**
- Ensure iRacing is running and connected
- Must be in Drive mode in the car
- Check that controls were scanned for this car
- Try scanning controls again

### Performance Issues

**Application is slow or laggy:**
- Close other background applications
- Check CPU/RAM usage in Task Manager
- Try reducing HUD update rate
- Ensure Windows is not in power-saving mode

---

## Updating to New Versions

When a new version is released:

1. **Download** the new release ZIP
2. **Extract** to the same location (overwrite files when asked)
3. **Your configurations are preserved** automatically
4. **Run** the new version
5. **Read** the changelog for new features

Your settings are stored separately, so they won't be lost.

---

## Uninstallation

If you need to remove the application:

### Remove Application Files
1. Close the application if running
2. Delete the extracted folder (e.g., `C:\iRacingControl\`)

### Remove Configuration Files (Optional)
1. Press `Win + R`
2. Type `%APPDATA%` and press Enter
3. Delete the `iRacingControlManager` folder

That's it - completely removed.

---

## Verification Checklist

After installation, verify:

- [ ] Application starts without errors
- [ ] Can connect to iRacing in practice session
- [ ] Scan detects vehicle controls
- [ ] Can configure keyboard keys
- [ ] HUD overlay appears and shows values
- [ ] Mode switching works (CONFIG ↔ RUNNING)
- [ ] Can save and load configurations
- [ ] Input devices are detected (if using controllers)

---

## Privacy & Security

This application:
- Does not require internet access (except iRacing telemetry)
- Does not collect or transmit any data
- Stores all settings locally
- Does not connect to external servers
- Does not track or monitor usage
- No analytics or telemetry

Your data stays on your computer.

---

## Important Reminders

### Appropriate Use
- ✅ Accessibility assistance
- ✅ Equipment limitations
- ✅ Educational learning
- ✅ Private practice sessions

### Inappropriate Use
- ❌ Competitive racing without proper justification
- ❌ Seeking unfair advantages
- ❌ Violating platform terms of service
- ❌ Public distribution or sharing

### Discretion Required
- Do not post about this publicly
- Do not create tutorials or videos
- Do not share on forums or social media
- Keep private and confidential

---

## Getting Help

For support:
- Review this guide thoroughly
- Check all documentation files
- Test extensively in private sessions
- Contact privately (no public forums)

**Remember**: Public discussion could draw unwanted attention and harm all legitimate accessibility users.

---

## Next Steps

After successful installation:
1. Read **README.md** for feature overview
2. Review **DISCLAIMER.md** for legal information  
3. Read **User Agreement** for responsible use guidelines
4. Start with private practice sessions only
5. Test thoroughly before any other use

**Use responsibly. Use ethically. Your choices matter.**
