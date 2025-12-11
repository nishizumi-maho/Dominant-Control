# Frequently Asked Questions (FAQ)

Common questions about Dominant Control for iRacing.

---

## General Questions

### What is this software?

This is an accessibility tool and educational application that provides an interface for managing vehicle settings in iRacing. It's designed to help drivers who:
- Have physical limitations that make reaching certain controls difficult
- Use equipment that lacks certain features (no rotary knobs, button boxes, etc.)
- Want to learn about telemetry systems and vehicle dynamics

### Who is this for?

**Primary Users:**
- Drivers with physical disabilities or mobility limitations
- Users with basic equipment lacking advanced features
- Students and educators learning about sim racing systems
- Hobbyists experimenting in private practice sessions

**Not For:**
- Seeking unfair competitive advantages
- Professional racing without proper justification
- Public competitive use without authorization

### Is this free?

The software is distributed to authorized users only. See distribution terms for details.

---

## Compliance & Legal

### Is this allowed by iRacing?

**Important**: We do not speak for iRacing. YOU are responsible for determining compliance.

iRacing's policy (8.1.1.2) states:
> "Exceptions may exist under iRacing's sole discretion for supporting accessibility features for disabled drivers or other reasons iRacing deems acceptable."

This tool is designed with accessibility needs in mind. However:
- **You must evaluate** if your situation qualifies
- **You are responsible** for ensuring compliant use
- **We provide no guarantees** about policy interpretation
- **Use at your own risk**

### Can I use this in official races?

**We strongly recommend:**
- ✅ Use only in private practice sessions
- ✅ Use for testing and learning
- ✅ Use with genuine accessibility needs

**Avoid:**
- ❌ Using in official competitions without clear justification
- ❌ Using to gain unfair competitive advantages
- ❌ Any use that violates platform policies

**Your responsibility** to ensure appropriate use.

### What if I get banned?

**We are not responsible** for any account actions, bans, or suspensions. 

You accept all risks when using this software. See DISCLAIMER.md for complete legal information.

### Can I ask iRacing support about this?

**We recommend:**
- Read all iRacing policies yourself
- Make your own informed decision
- If you have genuine accessibility needs, you can inquire about accommodation
- Be honest about your situation

**We do not recommend:**
- Asking specifically about this tool by name
- Drawing unnecessary attention
- Discussing in public forums

---

## Installation & Setup

### Do I need Python installed?

**No!** This is a standalone executable. Just download, extract, and run. No Python or dependencies required.

### Why does Windows block the application?

Windows SmartScreen blocks unrecognized apps without code-signing certificates (which cost thousands of dollars annually).

**To run:**
1. Click "More info"
2. Click "Run anyway"

The application is safe and contains no malware.

### Where are configurations stored?

```
%APPDATA%\iRacingControlManager\configs\
```

Your settings are stored separately from the application files.

### Can I use this on multiple computers?

The license covers personal use. You can install on your own computers, but:
- ❌ Do not share with others
- ❌ Do not distribute
- ❌ Keep private and confidential

---

## Usage Questions

### How do I start using this?

See **QUICKSTART.md** for a 5-minute setup guide.

**Basic steps:**
1. Extract the .exe to a folder
2. Run iRacingControlManager.exe
3. Start iRacing (private practice session)
4. Click "Scan Driver Controls"
5. Configure keys for each control
6. Switch to RUNNING mode
7. Test in private session

### Can I use my keyboard only?

**Yes!** The application works perfectly with keyboard-only input. Check "Keyboard Only Mode" in settings if you don't want to use controllers.

### Can I use wheel buttons?

Yes, but be selective. We recommend:
- ✅ Enable button boxes or separate controllers
- ❌ Don't enable your wheel device itself
- ❌ Don't enable pedals

Use the "Manage Devices" function to choose which devices to use.

### How do I create presets?

In any control tab:
1. Enter a target value (e.g., "52.5")
2. Click "Set Bind"
3. Press a keyboard key or controller button
4. Now that button jumps to that exact value

### What are combo macros?

Combos let you adjust multiple controls with **one button press**. For example:
- Wet setup: Set TC to 5, ABS to 3, Brake Bias to 54.0
- Dry setup: Set TC to 1, ABS to 0, Brake Bias to 52.5
- All with a single button!

Go to the "⚡ Combos" tab to set these up.

### Why isn't the HUD showing?

Check:
1. Options → Show/Hide Overlay (is it enabled?)
2. Go to "HUD / Overlay" tab - are variables checked?
3. Is opacity too low? (try 0.85)
4. Is it off-screen? (try dragging it)
5. Did you click in the application window first?

---

## Technical Questions

### I lost force feedback after opening the app! Help!

This is a known issue with Python's joystick handling library. **Solution:**

**Prevention (Best approach):**
1. Always open the app BEFORE starting iRacing
2. Then start iRacing
3. After sim loads, scan controls
4. Force feedback will work normally

**If already lost:**
1. Close iRacing completely
2. Restart iRacing (app can stay open)
3. Wait for sim to fully load
4. Should be back to normal

**Permanent fix:**
Enable **"Keyboard Only Mode"** in settings:
- Eliminates the issue completely
- Recommended if you only use keyboard keys for bindings
- No need to worry about startup order anymore

### What causes the force feedback issue?

This is a technical limitation of the joystick handling library used by the application (pygame). When it initializes device access after iRacing has already claimed the devices, conflicts can occur. 

**This is NOT a bug in the application** - it's an inherent limitation of how Python handles device access on Windows. The app must initialize device support before the sim does.

If you don't need wheel buttons or controller buttons (just keyboard), use Keyboard-Only Mode to bypass this entirely.

### Does this work with all cars?

It works with any car that has driver-adjustable controls. The "Scan Driver Controls" function detects what's available for each specific car.

Some cars have many adjustments (GT3, LMP2), others have few or none (street cars).

### Can I save different setups per track?

**Yes!** The application saves configurations per car AND per track combination. You can have:
- BMW M4 @ Spa
- BMW M4 @ Nurburgring
- Porsche 911 @ Spa
- Etc.

Each saves separately and auto-loads when detected.

### How fast are the adjustments?

Adjustable! Go to **Options → Timing Adjustments** and choose:
- **Aggressive**: Fast (40ms intervals)
- **Casual**: Medium (80-100ms)
- **Relaxed**: Slow (150-200ms)
- **Custom**: Define your own

### Does this read my iRacing password?

**No!** The application only connects to iRacing's telemetry API (same as any telemetry app like iSpeed, CrewChief, etc.). It:
- ✅ Reads telemetry data
- ✅ Sees vehicle parameters
- ❌ Cannot access login credentials
- ❌ Cannot access account information
- ❌ Does not connect to iRacing servers

### Does this send any data externally?

**Absolutely not!** This application:
- Does not connect to the internet (except iRacing's local telemetry)
- Does not transmit any data
- Does not collect analytics or telemetry
- Stores everything locally only
- Has no tracking or monitoring

100% offline and private.

---

## Accessibility Questions

### I have a physical disability. Is this appropriate for me?

If you have genuine physical limitations that prevent you from:
- Reaching certain controls on your wheel
- Performing rapid manual adjustments
- Using rotary knobs or complex controls

Then this tool may be appropriate as an **accessibility aid**. You should:
1. Evaluate your specific needs
2. Understand iRacing's accessibility exception policy
3. Use responsibly and ethically
4. Be prepared to explain your situation if asked

### My equipment doesn't have a rotary knob. Can I use this?

If your wheel lacks certain features (rotary adjustment knobs, button boxes, etc.), this tool can help compensate for that equipment limitation.

This is a legitimate use case - not all sim racers can afford $1000+ wheels with every feature.

### Do I need medical documentation?

**We don't require anything.** However:
- You should be honest with yourself about your use case
- If questioned by platform, you may need to explain your situation
- Have a genuine, honest reason for use
- Don't abuse the accessibility justification

---

## Privacy & Security

### Is my data safe?

Yes! Your data never leaves your computer:
- All configurations stored locally
- No internet connection (except iRacing telemetry)
- No external data transmission
- No cloud storage or backups
- Complete privacy

### Can other drivers detect this?

The application reads telemetry (like any telemetry app) and operates locally. It doesn't modify iRacing's memory or code.

However:
- Use discretion
- Don't discuss publicly
- Keep confidential
- Use responsibly

### Does iRacing see this running?

iRacing can detect active processes on your system. They use anti-cheat measures like any online game.

**Our stance:**
- This tool is designed for accessibility
- We operate transparently
- We encourage ethical use
- You are responsible for compliance

---

## Ethics & Responsibility

### Is using this considered cheating?

**Our position:**
- If used for genuine accessibility needs → No
- If used for educational purposes → No
- If used to circumvent fair play → Yes

**Your responsibility:**
- Evaluate your use case honestly
- Consider the spirit of competition
- Use ethically and responsibly
- Accept consequences of your choices

### Should I tell other people about this?

**We strongly recommend:**
- ❌ Do NOT post on forums or social media
- ❌ Do NOT create tutorials or videos
- ❌ Do NOT share screenshots showing the tool
- ❌ Do NOT distribute to others
- ✅ Keep private and confidential

Why? Public attention could:
- Result in countermeasures
- Harm legitimate accessibility users
- Draw scrutiny to everyone
- Violate the license terms

### What if someone asks me about my controls?

**Be honest:**
- If you have genuine accessibility needs, you can explain that
- If you lack certain equipment features, you can mention that
- Don't lie or make up disabilities
- Don't claim false justifications

**Be discreet:**
- Don't volunteer information unnecessarily
- Don't brag or show off
- Keep a low profile
- Respect the community

---

## Troubleshooting

### The application won't start

**Try:**
1. Ensure Windows 10/11 64-bit
2. Install Visual C++ Redistributable (from Microsoft)
3. Run as Administrator
4. Check Windows Defender didn't quarantine it
5. See INSTALLATION.md for detailed troubleshooting

### Controls aren't working in iRacing

**Check:**
1. Are you in RUNNING mode? (not CONFIG)
2. Are keys properly configured? (should show key names)
3. Is iRacing the active window?
4. Are you in a practice session (not menus)?
5. Did you save the configuration?

### It's adjusting too fast/slow

Go to **Options → Timing Adjustments** and:
- Try a different profile (Aggressive/Casual/Relaxed)
- Or use Custom to fine-tune specific timings

---

## Support

### How do I get help?

1. **Read all documentation** thoroughly first
2. **Check INSTALLATION.md** for troubleshooting
3. **Test extensively** in private sessions
4. **Contact privately** (never publicly)

### Can I request features?

Feature requests can be submitted privately. However:
- No promises or timelines
- Development priorities focus on accessibility and education
- Updates are discretionary
- Keep suggestions private

### Found a bug?

Report privately with:
- Version number
- Windows version
- Steps to reproduce
- Error messages or screenshots
- What you expected vs what happened

---

## Final Reminders

### Use Responsibly
This is a tool. Like any tool, it can be used well or poorly. **Your choices matter.**

### You Are Responsible
- For understanding policies
- For ensuring compliance
- For ethical use
- For all consequences

### Keep Private
- Don't publicize
- Don't distribute
- Don't share details
- Maintain confidentiality

### Use Ethically
- Genuine needs only
- Private sessions
- Respect fair play
- Honor the community

---

**Still have questions?** Review all documentation files, especially DISCLAIMER.md and LICENSE.md.

**Remember**: Your responsibility. Your choice. Use wisely.
