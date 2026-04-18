# 🛡️ Secure Data Recovery from RAT-Infected Android Device using Live USB

## 📌 Abstract

This project presents a real-world cybersecurity incident involving a Remote Access Trojan (RAT) infection on an Android device. The objective was to safely recover user data without spreading malware to another system. A Linux-based live environment was used to ensure isolation and security.

---

## 🚨 Incident Summary

A student downloaded and extracted an unknown file on his Android device, assuming it to be safe. However, the file contained a RAT.

Shortly after:

* Abnormal internet usage was observed
* Entire 5GB college Wi-Fi quota was consumed unexpectedly
* Suspicion of unauthorized remote access and data exfiltration arose

The issue was escalated after a cyber café refused to handle it due to risk.

---

## ⚠️ Threat Overview

* **Malware Type:** Remote Access Trojan (RAT)
* **Delivery Method:** Social engineering (disguised file)
* **Capabilities:**

  * Remote device access
  * Data exfiltration
  * Network abuse
  * Background execution

---

## 🎯 Objectives

* Extract important user data safely
* Avoid malware execution
* Prevent infection of host system
* Maintain data integrity

---

## 💡 Solution Strategy

A secure and isolated environment was created using a Linux Live USB.

### Why Ubuntu Live?

* Runs in RAM (non-persistent)
* Does not affect host OS
* Ideal for forensic and recovery tasks

---

## ⚙️ Methodology

### Step 1: Environment Preparation

* Downloaded Ubuntu ISO
* Created bootable USB using Rufus

### Step 2: Secure Boot Execution

* Booted system using USB
* Selected “Try Ubuntu” (Live Mode)
* Disabled internet connectivity

### Step 3: Controlled Device Access

* Connected infected Android device via USB
* Enabled file transfer (MTP mode)

### Step 4: Data Extraction

* Accessed storage without executing files
* Copied required data to a separate clean USB

### Step 5: Safe Exit

* Unmounted all devices
* Shut down system
* Removed USB devices

---

## 🔒 Security Controls Implemented

* Air-gapped environment (no internet)
* No file execution policy
* Read-only interaction mindset
* No mounting of internal drives
* Temporary OS usage

---

## ⚠️ Risk Analysis & Mitigation

| Risk              | Impact            | Mitigation                    |
| ----------------- | ----------------- | ----------------------------- |
| Malware execution | System compromise | Avoided opening files         |
| Data leakage      | Privacy breach    | Offline environment           |
| USB infection     | Spread of malware | No execution + scanning later |
| System damage     | OS corruption     | Live OS usage                 |

---

## 📊 Workflow Diagram

(Add diagram in diagrams/workflow.png)

---

## 🧠 Key Learnings

* Human error is the weakest security link
* Isolation is the strongest defense
* Live OS can act as a forensic tool
* Never trust unknown files

---

## 🚀 Future Enhancements

* Automated malware detection integration
* Sandboxed file analysis
* Network traffic monitoring tools
* Incident response playbook development

---

## ⚠️ Disclaimer

This project is intended for educational and ethical cybersecurity purposes only. No personal or sensitive data has been shared.

---

## 📎 Tags

`Cybersecurity` `Digital Forensics` `Malware Analysis` `Linux` `Incident Response`
