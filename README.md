# Home Technology Runbook

> **For: Non-technical caretaker / house-sitter**  
> **Owner: Neko**  
> **Purpose:** Maintain, troubleshoot, and manage the residential network and streaming setup in Neko's home during absence (1–5 months)

---

## Table of Contents

1. [Glossary of Terms](#glossary-of-terms)  
2. [Device Overview](#device-overview)  
3. [Physical Locations](#physical-locations)  
4. [Restarting Wi-Fi & Troubleshooting Internet](#restarting-wi-fi--troubleshooting-internet)  
5. [Adding or Resetting Devices](#adding-or-resetting-devices)  
   - Roku TVs  
   - Apple TV  
   - Chromecast  
   - Amazon Echo Devices  
6. [Accessing NAS Storage](#accessing-nas-storage)  
7. [Using Proton Pass](#using-proton-pass)  
8. [Monthly Health Checklist](#monthly-health-checklist)  

---

## Glossary of Terms

- **Wi-Fi**: Wireless internet  
- **Router**: Directs all home internet traffic  
- **Switch**: Extends Ethernet ports to other rooms  
- **Access Point (AP)**: Wi-Fi broadcasting device  
- **SSID**: Wi-Fi network name  
- **NAS**: Network storage system (Synology DS1825+)  
- **Proton Pass**: Password manager with vault access to all credentials  
- **Ziggy**: Wake word for all Echo devices  

---

## Device Overview

### Networking
- **Ubiquiti Dream Machine Pro (UDM Pro)** – main router and UniFi controller  
- **Ubiquiti US-8-60W Switches (x5)** – network switches powering APs and hardwired devices  
- **Ubiquiti APs**  
  - U7 Pro Wall (x2)  
  - U7 Outdoor (x1)  
  - UAP Long Range (x4)  

### Entertainment & Smart Home
- **Roku TVs** – 65" Sharp and 50"  
- **Apple TV 4K** – used for HomeKit (do not modify automations)  
- **Chromecast 4K** – casting from phones  
- **Amazon Echo Devices**  
  - Echo Show 15" (x2)  
  - Echo Show 8" (x3)  
  - Echo Pop (x3)  
  - **Wake Word**: "Ziggy"  

### Storage
- **Synology DS1825+ NAS** – general storage and backups  

### Credentials
- **Proton Pass**: Everything lives in the vault named **"Heathens"**

---

## Physical Locations

_Note: Update with actual locations before leaving._

- UDM Pro: `______`  
- Switches #1-5: `______`  
- APs: `______`  
- NAS: `______`  
- Roku TVs: `______`  
- Apple TV: `______`  
- Chromecast: `______`  
- Echo Shows and Pops: `______`  

---

## Restarting Wi-Fi & Troubleshooting Internet

1. **Check Router LED (UDM Pro)**:  
   - Blue = OK  
   - Flashing Blue = No internet  
   - White = Booting or offline  

2. **Check Modem**:  
   - All lights green = Good  
   - Reboot if red/off (power off 10 sec, back on)  

3. **Check Switches & APs**:  
   - LEDs on = Good  
   - LED off = Likely offline (power cycle)  

4. **Restart Devices**:  
   - UDM Pro: Graceful via LCD or power cycle  
   - Switch: Unplug power, 10 sec, plug back  
   - AP: Unplug PoE cable for 10 sec  

5. **Test Internet**:  
   - Load website on phone/laptop  
   - Ask Ziggy something  

---

## Adding or Resetting Devices

### Roku TV
- **Menu Path**: Settings > Network > Set up Connection > Wireless  
- Select Wi-Fi > Enter Password  
- Test with Netflix or YouTube  
- Restart: Settings > System > Power > System Restart  

### Apple TV
- **Menu Path**: Settings > Network > Wi-Fi  
- Choose network > Enter password  
- Restart: Settings > System > Restart  

### Chromecast
- Use **Google Home App** > Add Device  
- Follow on-screen pairing  
- Use Proton Pass for Wi-Fi credentials  
- To reset: Hold button on Chromecast for 10 sec  

### Amazon Echo Devices
- Wake word: **"Ziggy"**  
- Update Wi-Fi: Alexa app > Devices > [Your Echo] > Wi-Fi Network  
- Echo Show: Swipe down > Settings > Network  
- Reset: Mute + Volume Down (Show), Volume Down + Mic Off (Pop)  

---

## Accessing NAS Storage

### Windows:
- File Explorer > Network > DiskStation (or)  
- Map Network Drive: `\\NAS_NAME\\Share`  
- Login with Proton Pass credentials  

### Mac:
- Finder > Go > Connect to Server > `smb://NAS_NAME` or IP  
- Login as above  

### Web Interface:
- Browser > `http://<NAS_IP>:5000`  
- Login > File Station app for drag/drop  

> ⚠️ Do not modify advanced NAS settings  

---

## Using Proton Pass

1. **Install Proton Pass**  
   - Mobile app or browser extension  

2. **Login**  
   - Use Proton account credentials (stored securely)  
   - Access vault **"Heathens"**  

3. **Retrieve Passwords**  
   - Search for: Wi-Fi, Roku, NAS, Amazon, etc.  
   - Click to reveal/copy as needed  

4. **Security Notes**  
   - Never write down passwords elsewhere  
   - Update vault if you change any credentials  

---

## Monthly Health Checklist

- ✅ UDM Pro LED = Solid Blue  
- ✅ All switches powered & active ports blinking  
- ✅ APs lit & reachable via Wi-Fi  
- ✅ NAS = Status LED Green, drive LEDs green/blinking  
- ✅ Alexa devices respond to “Ziggy”  
- ✅ Roku, Apple TV, Chromecast working  
- ✅ Speedtest OK, normal browsing/streaming  
- ✅ NAS reachable from PC/Mac  
- ✅ No strange beeps, red lights, overheating  
- ✅ Cables secure, no physical damage  

---

## Final Notes

- For any tasks not covered here (like HomeKit automations), **leave them alone**.  
- If something major breaks and you can't fix it via this guide, document what happened and leave it for the owner.  
- Keep this document saved and printed.  
- Proton Pass is your lifeline—**everything you need is in the Heathens vault**.  

Stay calm, take your time, follow the steps, and you’ll be fine.

---

**End of Runbook**
