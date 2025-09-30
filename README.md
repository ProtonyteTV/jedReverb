# 🎧 jedReverb 25.0

**Level up your audio with powerful, real-time effects and high-quality offline rendering.**

jedReverb is a modern audio processing application for iOS and iPadOS. Built with **SwiftUI** and **AVFoundation**, it allows you to import audio files, apply a suite of creative effects—like **Reverb**, **Pitch Shift**, and **Rate Change**—and then export the final, processed track.

## ✨ Features at a Glance

* **Real-Time Effects Engine:** Manipulate effects in real-time with a stable, professional-grade `AVAudioEngine` pipeline.
* **Offline Rendering:** Save your processed audio as a high-quality M4A file, ensuring perfect application of all effects, regardless of playback complexity.
* **Intuitive Controls:** Fine-tune every effect parameter (Pitch, Rate, Reverb, Bass Boost) using a clean, native **SwiftUI** interface.
* **Instant Presets:** Quickly apply popular sound styles like **"Slowed + Reverb"** and **"Nightcore"** with dedicated buttons.
* **Full Customization:** Personalize your app experience with user-selectable **Themes** (System, Light, Dark) and **Accent Colors**.

## 🛠️ Requirements

* **iOS 14 and Later**

## 🚀 How to Use

1.  **Import:** Tap the **"Import Audio"** button to select a music file, voice memo, or any standard audio format from your device's files.
2.  **Tweak:** Adjust the sliders in the **Effects Card** section to hear the changes immediately in real-time.
3.  **Preview:** Use the main control button to **Play** and **Pause**. The **Time Scrubber** allows you to navigate the audio instantly.
4.  **Export:** When you are happy with the result, tap **"Save Audio"**. The app will perform a background **Offline Render**, and then present a share sheet for you to save the new M4A file to your device or share it.

## 💻 Technical Overview (For Developers/Auditors)

| Component | Technology | Role in Project |
| :--- | :--- | :--- |
| **Interface** | SwiftUI | Clean, declarative UI using custom view components. |
| **Audio Core** | AVFoundation | Manages `AVAudioEngine`, audio unit effects, and complex offline rendering. |
| **State Management** | Combine, MVVM | Used for reactive updates and synchronizing UI state with the low-level audio engine. |
| **Configuration** | Managers (Theme, Color) | Singleton objects handling app-wide persistence for settings via `UserDefaults`. |
