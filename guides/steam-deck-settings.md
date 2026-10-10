---
title: "Steam Deck 60FPS Lock Guide: Optimal Graphics, TDP & Battery Calibration"
description: "Eliminate frame stutter and fan noise in Nivalis. Hand-tested Steam Deck presets for locked 60FPS, battery-saving 40Hz mode, and FSR 2.0 sharpness settings."
category: "Tech & Performance"
badge: "VERIFIED STEAM DECK OLED & LCD"
readingTime: "5 min read"
publishDate: "2026-03-20"
lang: "en"
---

## 1. Verified Steam Deck Performance Presets

Nivalis features dense cyberpunk geometry, dynamic neon lighting, and complex volumetric rain reflections that can stress handheld hardware if unoptimized.

We tested dozens of parameter combinations on both **Steam Deck LCD** and **Steam Deck OLED** to establish two recommended presets:

| Setting Category | Preset A: Smooth 60 FPS (Plugged-In / High Smoothness) | Preset B: 40Hz / 40 FPS (Battery Saver: 3.5h Playtime) |
| :--- | :--- | :--- |
| **Resolution** | 1280 x 800 (Native) | 1280 x 800 (Native) |
| **FSR Scaling** | FSR 2.0 Balanced | FSR 2.0 Quality |
| **Volumetric Rain & Fog** | Medium | Low |
| **Screen Space Reflections** | Medium | Off |
| **Shadow Resolution** | Medium | Low |
| **Crowd Density** | High | Medium |
| **SteamOS Refresh Rate** | 60 Hz | 40 Hz |
| **Frame Limit** | 60 FPS | 40 FPS |
| **TDP Limit** | 12 Watts | 10 Watts |
| **GPU Clock Lock** | Manual: 1200 MHz | Auto |

---

## 2. In-Game Graphics Settings Walkthrough

To apply these settings:
1. Open the pause menu and navigate to **Settings &rarr; Display & Graphics**.
2. Set **Motion Blur** to **Off** (significantly reduces visual ghosting in fast canal motorboat turns).
3. Set **V-Sync** to **Off** inside the game engine; allow the **SteamOS compositor** to handle frame pacing directly to eliminate input lag.
4. Set **Dynamic Resolution Scaling** to **Target 60 FPS**.

---

## 3. SteamOS Quick Access Overlay Tweaks

Press the **"..." (Quick Access)** button on the right side of your Steam Deck:
- Enable **Advanced View** in the Performance tab.
- Set **Scaling Filter** to **FSR** with Sharpness set to **3**.
- Set **TDP Limit** to **11W** (this prevents aggressive CPU throttling and eliminates fan noise without causing frame drops in dense nightclub interiors).

---

## 4. Trackpad & Gyro Angling Control Scheme

For the best fishing and boat navigation experience:
- Set the **Right Trackpad as Mouse** with low sensitivity for precision menu navigation.
- Configure **Gyro Aiming (As Mouse)** activated on **Left Trigger Soft Pull** to assist with fine line tension adjustments during trophy fish battles.
