# Privacy Policy for Wavegod Spatial

**Effective Date:** January 22, 2025
**Version:** 1.1

---

## Overview

Wavegod Spatial ("we", "our", or "the app") is committed to protecting your privacy. This Privacy Policy explains how we handle your information when you use our iOS application.

**Simple Summary:** We don't collect, store, or transmit any of your personal data. Everything stays on your device.

---

## Information Collection and Use

### What We DON'T Collect

Wavegod Spatial does **NOT** collect, store, or transmit:

- ❌ Personal information (name, email, phone number)
- ❌ Location data
- ❌ Usage analytics or statistics
- ❌ Crash reports
- ❌ Device identifiers
- ❌ IP addresses
- ❌ Any other personal or identifying information

### What Data the App Processes (On-Device Only)

The app processes the following data **locally on your device only**:

1. **Motion Sensor Data**
   - Gyroscope readings
   - Accelerometer readings
   - Compass/magnetometer readings
   - This data is used in real-time to generate MIDI and OSC messages
   - **Not stored, not transmitted to us, not logged**

2. **UWB (Ultra-Wideband) Spatial Data**
   - Distance and direction measurements between nearby devices
   - Used for precise spatial positioning in collaborative mode
   - Processed locally, transmitted only to connected devices on local network
   - **Not stored permanently, not sent to external servers**

3. **User Settings**
   - MIDI configuration (channel, CC mappings, note range)
   - OSC configuration (host IP, port, update rate)
   - App preferences (smoothing, calibration settings)
   - Stored locally on your device using iOS UserDefaults
   - Optionally synced via your personal iCloud account (see below)

4. **Premium/Trial Status**
   - Trial start date and expiration (14-day trial period)
   - Premium unlock purchase status
   - Stored locally and synced via iCloud for multi-device access
   - Purchase verification handled by Apple's StoreKit 2
   - **We do not have access to your payment information**

---

## iCloud Sync (Optional)

Wavegod Spatial offers **optional** iCloud sync for your settings:

- **What's synced:** Only your app settings (MIDI/OSC configuration, preferences)
- **Where it's stored:** Your personal iCloud account (controlled by you)
- **Who has access:** Only you (via your Apple ID)
- **We do NOT have access** to your iCloud data
- **You can disable** iCloud sync at any time in Settings

iCloud sync is handled entirely by Apple's CloudKit framework. We do not have access to, and cannot see, your iCloud data.

---

## Local Network Usage

Wavegod Spatial uses your **local network** for the following purposes:

### MIDI Output
- Sends MIDI messages to music software on your Mac/iPad/PC
- Uses standard MIDI protocols (Core MIDI, Network MIDI)
- Only sends musical control data (notes, CC values)
- Transmitted over your local WiFi network only

### OSC Output
- Sends OSC (Open Sound Control) messages to visual software
- Uses UDP protocol on your local network
- Only sends spatial data (azimuth, elevation, distance)
- Optionally supports broadcast/multicast for device discovery
- Never connects to the internet

**All network communication stays within your local network. The app does not connect to external servers.**

---

## Permissions Required

The app requests the following iOS permissions:

### Motion & Orientation (Required)
- **Purpose:** Read gyroscope, accelerometer, and compass data to generate MIDI/OSC output
- **Usage:** Real-time processing only, not stored

### Local Network Access (Required)
- **Purpose:** Send MIDI and OSC messages to software on your local network
- **Usage:** Communication with DAWs, visual software, and macOS Receiver app

### Nearby Interaction / UWB (Required for UWB Mode)
- **Purpose:** Measure precise distance and direction between devices using Ultra-Wideband
- **Usage:** Spatial positioning in collaborative mode with multiple devices
- **Note:** Only works on iPhone 11 and later with U1 chip

### Bluetooth (Required for UWB Mode)
- **Purpose:** Device discovery and UWB session establishment
- **Usage:** Finding and connecting to nearby devices for spatial collaboration
- **Note:** We do not collect Bluetooth device information

### Camera (Optional for UWB Mode)
- **Purpose:** Provide directional information for UWB measurements
- **Usage:** Enhanced accuracy for spatial positioning
- **Note:** Camera is not used for recording; only for directional assistance

### Location When In Use (Required for UWB Mode)
- **Purpose:** iOS requires location permission for UWB functionality
- **Usage:** We do NOT track your location; this is an iOS requirement for UWB
- **Note:** Your actual location is never collected, stored, or transmitted

### Background Modes (Optional)
- **Purpose:** Continue sending MIDI/OSC data when app is in background
- **Usage:** Maintains active MIDI/OSC session during multitasking

All permissions are used **only for the stated purposes** and never to collect data about you.

---

## Data Security

Since we don't collect any data, there is no data to secure or protect from breaches.

All settings are stored securely:
- Locally on your device using iOS secure storage
- In your personal iCloud account (if iCloud sync enabled)
- Protected by your device passcode and Apple ID

---

## Third-Party Services

Wavegod Spatial does **NOT** use any third-party services:

- ❌ No analytics services (Google Analytics, Mixpanel, etc.)
- ❌ No crash reporting (Crashlytics, Sentry, etc.)
- ❌ No advertising networks
- ❌ No social media integration
- ❌ No external payment processors

The only Apple services used:
- ✅ StoreKit 2 (for in-app purchases and trial management)
- ✅ CloudKit (optional, for syncing settings and premium status via your iCloud)
- ✅ Core MIDI (for MIDI output)
- ✅ Core Motion (for sensor data)
- ✅ Nearby Interaction (for UWB spatial positioning)
- ✅ MultipeerConnectivity (for device discovery)

These are standard iOS frameworks and do not transmit data to us. Purchase information is handled securely by Apple's infrastructure, and we never have access to your payment details.

---

## Children's Privacy

Wavegod Spatial does not collect any information from anyone, including children under the age of 13. The app is rated 4+ and is safe for all ages.

---

## Changes to This Privacy Policy

We may update this Privacy Policy from time to time. We will notify you of any changes by:
- Posting the new Privacy Policy in the app
- Updating the "Effective Date" at the top
- (For significant changes) Prompting you in the app

Your continued use of the app after changes constitutes acceptance of the updated policy.

---

## Your Rights

Since we don't collect any data about you, there is no data to:
- Access
- Delete
- Correct
- Export
- Restrict processing of

All your data stays on your device and in your personal iCloud account (if enabled).

---

## Contact Us

If you have questions about this Privacy Policy, please contact us:

**Email:** [Timo.Aula@boethius.fi](mailto:Timo.Aula@boethius.fi)
**GitHub:** [https://github.com/TipiusMaximus/wavegod-spatial-docs](https://github.com/TipiusMaximus/wavegod-spatial-docs)

---

## Compliance

This Privacy Policy complies with:
- Apple App Store Review Guidelines
- General Data Protection Regulation (GDPR) - EU
- California Consumer Privacy Act (CCPA) - USA
- Children's Online Privacy Protection Act (COPPA) - USA

**Data Controller:** Timo Aula
**Contact:** Timo.Aula@boethius.fi

---

## Summary

**TL;DR:**
- ✅ We don't collect any data about you
- ✅ Everything stays on your device
- ✅ Optional iCloud sync uses your personal iCloud
- ✅ Local network used only for MIDI/OSC output
- ✅ No third-party services
- ✅ No tracking, no analytics, no ads

**Your privacy is 100% protected because we simply don't collect any data.**

---

**Last Updated:** January 22, 2025
**Version:** 1.1
**App Version:** 1.0

---

## Legal

This Privacy Policy constitutes a legal agreement between you (the user) and Timo Aula (the developer). By downloading, installing, or using Wavegod Spatial, you agree to the terms of this Privacy Policy.

If you do not agree with this Privacy Policy, please do not use the app.

---

**Privacy Policy URL for App Store Connect:**

`https://tipiusmaximux.github.io/wavegod-spatial-docs/privacy`
