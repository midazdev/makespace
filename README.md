# 🚀 Midaz MakeSpace
### *Free up space without deleting your photos.*

<p align="center">
  <a href="https://makespace.midaz.dev">
    <img src="https://img.shields.io/badge/🚀%20Live%20App-makespace.midaz.dev-00f5d4.svg?style=for-the-badge&logo=googlechrome&logoColor=black" alt="Live Web App" />
  </a>
  <a href="https://github.com/midazdev/makespace">
    <img src="https://img.shields.io/badge/⭐%20Star%20Repo-makespace-fee440.svg?style=for-the-badge&logo=github&logoColor=black" alt="Star Repository" />
  </a>
  <a href="https://github.com/midazdev">
    <img src="https://img.shields.io/github/followers/midazdev?style=for-the-badge&logo=github&label=Follow%20%40midazdev&color=181717" alt="Follow on GitHub" />
  </a>
  <a href="https://www.linkedin.com/in/datosamuel">
    <img src="https://img.shields.io/badge/💼%20Connect-LinkedIn-0a66c2.svg?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Privacy-100%25%20On--Device%20(Zero%20Uploads)-brightgreen.svg?style=flat-square" alt="100% On-Device Privacy" />
  <img src="https://img.shields.io/badge/Engine-WebAssembly%20%2B%20HTML5%20Canvas-blueviolet.svg?style=flat-square" alt="WebAssembly Engine" />
  <img src="https://img.shields.io/badge/Apple%20HEIC-Supported%20🍏-orange.svg?style=flat-square" alt="Apple HEIC Supported" />
  <img src="https://img.shields.io/badge/PWA-Installable%20Offline-cyan.svg?style=flat-square" alt="PWA Installable" />
  <img src="https://img.shields.io/badge/License-PolyForm%20Noncommercial-red.svg?style=flat-square" alt="Non-Commercial License" />
  <img src="https://img.shields.io/badge/Cost-100%25%20Free%20Forever-success.svg?style=flat-square" alt="100% Free Forever" />
</p>

---

> [!TIP]
> **Launch Live Web App Directly in Browser**: Try MakeSpace on your iPhone, Android, Mac, or Windows PC at **[https://makespace.midaz.dev](https://makespace.midaz.dev)**. Zero sign-up, zero ads, 100% free!

---

## 📱 Is Your Phone Storage Almost Full?

<div align="center">

| 🚨 **The Old Way** | ✨ **The MakeSpace Way** |
| :--- | :--- |
| ❌ Pay **$2.99 – $9.99/month** for recurring cloud storage | ✅ **100% Free Forever** with zero subscription fees |
| ❌ Delete precious memories & holiday photos to free up space | ✅ **Keep all your photos** and reclaim up to **85% free space** |
| ❌ Upload private family photos to third-party servers | ✅ **100% On-Device Privacy** — zero bytes leave your browser RAM |
| ❌ Browser freezes when uploading 500+ heavy camera photos | ✅ **Smart Memory Slicing** handles hundreds of photos smoothly |

</div>

---

## 📊 Real-World Space Reclaimed Benchmark

Converting uncompressed camera photos into modern **WebP** shrinks file weight dramatically with **virtually zero human-perceptible visual loss**:

| Format & Source | Original Size | WebP (80% Sweet Spot) | Space Saved |
| :--- | :---: | :---: | :---: |
| 🍏 **iPhone 15 Pro HEIC** | `4.8 MB` | **`620 KB`** | **🔥 -87%** |
| 📸 **Android Camera JPG** | `6.2 MB` | **`780 KB`** | **🔥 -87%** |
| 🎨 **Heavy Screenshot / PNG** | `3.4 MB` | **`410 KB`** | **🔥 -88%** |
| 📁 **Holiday Album (100 Photos)** | `580 MB` | **`68 MB`** | **🎉 +512 MB Free Space!** |

---

## 🌟 Key Superpowers

### 🔒 1. 100% On-Device Privacy Guarantee
Zero tracking, zero analytics on your files, and zero cloud storage uploads. Every single photo is transcoded directly in your computer or smartphone's local RAM and WebAssembly. **No server ever sees or stores your images or photos.**

### 🍏 2. Apple HEIC / HEIF WebAssembly Engine
iPhones capture photos in proprietary `.heic` format. MakeSpace includes an embedded in-browser WebAssembly decoder that seamlessly converts `.heic` directly into universally compatible `.webp` files.

### 🎚️ 3. Smart Memory Slicing (Anti-Freeze Batching)
Compressing 200+ high-res photos at once can crash phone browsers. MakeSpace slices heavy queues into smart micro-batches (50 / 100 / 200) with a live progress HUD and memory garbage-collection checkpoints.

### 🧠 4. Tab Crash Recovery & Session Resume
Accidentally refreshed the tab or lost battery midway? MakeSpace automatically saves your session checkpoints in local storage, allowing you to resume right where you left off with 1 click.

### 📁 5. Auto Folder Naming & Direct PC Folder Saving
- Upload an entire folder named `holiday2026` ➔ Download is automatically named `holiday2026-optimized-webp.zip`.
- Original filenames are preserved cleanly (`bali1.jpg` ➔ `bali1.webp`).
- **Desktop Chrome / Edge**: Features **`📁 Save Directly to PC Folder`** using the *File System Access API* — writes all WebP photos directly to your hard drive without needing to unzip!

### 📲 6. Installable Offline PWA
Install MakeSpace as a standalone app on your iPhone (via *Safari ➔ Add to Home Screen*) or Android / Windows / Mac desktop for fast 1-tap offline access.

---

## 🎯 How to Use (3 Simple Steps)

```text
  [ 1. Select Photos ] ──────► [ 2. Pick Quality & Go ] ──────► [ 3. Download Results ]
  (Drop photos / folder)        (80% Sweet Spot • 1-Click)       (ZIP or Direct to Folder)
```

1. **Open the Web App**: Navigate to **[makespace.midaz.dev](https://makespace.midaz.dev)** on your phone or PC.
2. **Select Photos**: Drag & drop photos, click *Select Photos (Multi-Select)*, or *Select Entire Folder*.
3. **Reclaim Space**: Choose your quality profile (default: `80% Sweet Spot`) and click **✨ Reclaim Space Now**.
4. **Download**: Hit **`📦 Download .ZIP Archive`** or **`📁 Save Directly to PC Folder`** and enjoy your free space!

---

## 🛠️ Architecture & Tech Stack

```text
  ┌─────────────────────────────────────────────────────────────┐
  │                    MIDAZ MAKESPACE ENGINE                   │
  │                                                             │
  │   [ Raw Photos ] ──► [ heic2any WASM ] ──► [ Canvas API ]  │
  │   (HEIC/JPG/PNG)         (Apple Decoder)     (WebP Encoder) │
  │                                                    │        │
  │   [ Direct to Folder ] ◄── [ JSZip Stream ] ◄──────┘        │
  │   (File System API)        (ZIP Packaging)                  │
  └─────────────────────────────────────────────────────────────┘
```

* **Frontend Architecture**: React 18, TypeScript, Tailwind CSS, Lucide Icons, Vite
* **Transcoding Engine**: HTML5 Canvas 2D API + `heic2any` WebAssembly
* **Archiving & File System**: `JSZip` + W3C File System Access API
* **State & Persistence**: LocalStorage Session Store + URL Object Blobs
* **Production Deployment**: Cloudflare Edge Infrastructure (`makespace.midaz.dev`)

---

## 👨‍💻 Creator & Engineering Credits

Crafted with ❤️ by **Dato' Samuel F.**  
*Founder & Principal AI Systems Architect* at **Midaz Dev**.

* 🌐 **Live Interactive Portfolio**: [samuel.midaz.dev](https://samuel.midaz.dev)
* 💼 **LinkedIn**: [linkedin.com/in/datosamuel](https://www.linkedin.com/in/datosamuel)
* 🐙 **GitHub Profile**: [github.com/midazdev](https://github.com/midazdev)
* 📧 **Direct Inquiries**: `samuel@midaz.dev`

---

## ⭐ Show Your Support & Stay Updated

If Midaz MakeSpace saved you from paying cloud storage subscriptions or freed up space on your phone:

1. **⭐ Star this repository** on GitHub: [github.com/midazdev/makespace](https://github.com/midazdev/makespace)
2. **👤 Follow the creator** on GitHub: [github.com/midazdev](https://github.com/midazdev) for upcoming open-source tools
3. **💼 Connect on LinkedIn**: [linkedin.com/in/datosamuel](https://www.linkedin.com/in/datosamuel)
4. **🔗 Share with friends**: [makespace.midaz.dev](https://makespace.midaz.dev)

---

## 📜 License & Legal Terms

This application is provided **100% free of charge for personal use**.  
Protected under the **[PolyForm Noncommercial License 1.0.0](LICENSE)**. 

* **Permitted**: Personal use, evaluation, study, and direct web application access.
* **Strictly Prohibited**: Commercial redistribution, reselling, rebranding, white-labeling, or deployment as a commercial paid service without prior written consent from the author.

© 2026 **Dato' Samuel F. | Midaz Dev**. All rights reserved.
