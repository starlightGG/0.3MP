# 0.3MP Video Station 📹

**Turn your modern high-res camera into a 2004 flip-phone masterpiece.**

0.3MP Video Station is a browser-based application that simulates the aesthetic of early camera phones (VGA/0.3 Megapixel era) and VHS tapes. It features a custom-built rendering pipeline for authentic digital decay, including spatial RGB channel separation, LCD ghosting, JPEG compression artifacts, and telephony-grade audio processing.

**No subscriptions. No watermarks. Just pure digital nostalgia.**

## ✨ Features

### 📸 Visual Engine
* **Phone Profiles:** Emulations of specific devices including Nokia 7650, Moto Razr, Sony K750, Siemens, Sharp GX, and more.
* **Spatial RGB Outline:** A custom "Holographic" edge effect that separates Red and Blue channels spatially (not just temporal lag).
* **LCD Ghosting:** Simulates the slow response time of early color LCD screens with a dedicated lag trail slider.
* **Compression & Crunch:** Dynamic sliders for `Contrast/Crush` (dynamic range) and `Compression/Quality` (banding and block artifacts).
* **Digital Zoom:** Authentic, pixelated digital zoom logic.

### 🔊 Audio Engine
* **Telephony Filters:** Uses Web Audio API `BiquadFilterNode` (High-pass & Low-pass) to replicate the narrow 300Hz-3400Hz bandwidth of old microphones.
* **Distortion & Saturation:** Custom WaveShaper curves to simulate cheap analog pre-amps clipping.
* **Background Noise:** Generative noise floor (hiss) that "pumps" with the compressor to simulate early Automatic Gain Control (AGC).

### 🛠 Tools
* **Import Wizard:** Process existing Videos or Photos through the engine.
* **Smart Export:** Download processed media as WebM (video) or JPG/PNG (photos).
* **Custom UI Overlay:** Customizable on-screen text (e.g., "VGA FINE", "READY") and battery indicator logic.
* **Selfie Mode:** Flip between Environment (Rear) and User (Front) cameras.

## 🚀 How to Run

Since this is a single-file application, running it is incredibly simple:

1.  Download the `index.html` file.
2.  Open it in any modern web browser (Chrome, Safari, Firefox, Edge).
3.  Click **"TAP TO START"** to initialize the AudioContext and Camera permissions.
*(You could also open [StarlightGG 0.3MP](https://starlightgg.github.io/0.3MP) to run it)*

*Note: For the best experience on mobile, add the page to your Home Screen to run it in fullscreen mode.*

## 🎛 Controls Guide

| Control | Function |
| :--- | :--- |
| **DIGITAL ZOOM** | Crops and scales the image. Low values = Wide, High values = Pixelated Zoom. |
| **BLUR** | Adds an optical blur before processing (simulates dirty lens/bad focus). |
| **RGB OUTLINE** | Controls the spatial distance between Red and Blue channels. Higher = wider separation. |
| **LCD GHOSTING** | Controls screen persistence. Higher = longer trails and motion blur. |
| **CONTRAST** | Left = Flat/Washed out. Right = Crushed blacks and blown-out whites. |
| **QUALITY** | Left = Smooth. Right = Heavy banding and grid artifacts. |

## 📱 Supported Modes

* **NOKIA 7650:** Green tint, noisy, heavy banding.
* **MOTO RAZR:** Blue tint, high contrast, crushed blacks.
* **SONY K750:** Warm, soft, bloom-like quality.
* **SIEMENS:** Yellow/Green tint, heavy audio distortion.
* **SHARP GX:** Clean but digital look.
* **SAMSUNG:** Balanced, slight magenta shift.
* **LG FLIP:** Cold, washed out.
* **PALM TREO:** High saturation, distinct compression.
* **SENSOR RAW:** Debug mode with adjustable pure RGB separation.
* **VHS TAPE:** Interlaced scanlines, tracking noise, warm color profile.

## 📄 License

Open Source. Feel free to modify, distribute, and use for your own aesthetic projects.
