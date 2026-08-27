# RetroLens Mobile & Desktop 🖐️✨

**Real-time hand tracking portal filter** - Works perfectly on **HP, Tablet, and Laptop!**

Streamlit version untuk kemudahan akses dari HP dan Desktop tanpa perlu install banyak dependencies.

---

## 🚀 **RUN INSTANTLY - Click Button Below!**

### ⭐ **CLICK HERE TO RUN ONLINE (No Installation Needed!)**

[![Open in Streamlit Cloud](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://retrolens-mobile-mahar.streamlit.app)

👆 **Just click above and start using immediately on your HP or Laptop!** ✨

---

## 🌟 Features

- ✅ **Live Camera** - Real-time hand gesture tracking
- ✅ **Video Upload** - Process video files with filters
- ✅ **11 Filters** - Dual-tone, Thermal, Sketch, Pixelate, Glitch, Invert, Red-channel, Edge, Blur, Cartoon, Rainbow-wave
- ✅ **2D/3D Mode** - Toggle between different gesture detection modes
- ✅ **Mobile Responsive** - Perfect on HP, Tablet, and Laptop
- ✅ **No Installation** - Runs directly from browser
- ✅ **Real-time Settings** - Adjust sensitivity on-the-fly

---

## 💻 Run Locally (Optional)

### Install

```bash
git clone https://github.com/mahar-debug/Retrolens-Mobile.git
cd Retrolens-Mobile
pip install -r requirements_streamlit.txt
```

### Run on Desktop/Laptop

```bash
streamlit run streamlit_app.py
```

Browser will open at: `http://localhost:8501`

### Access from Mobile Phone (Same WiFi)

1. **On Laptop**, run the command above
2. **Find the IP address** shown in terminal (e.g., `192.168.1.100`)
3. **On Phone**, open browser: `http://192.168.1.100:8501`
4. Tap **"📹 Live Camera"** and allow camera access
5. **Start using!**

---

## 📱 Cara Menggunakan (Indonesian)

### 🎯 LANGSUNG BUKA DI BROWSER

Klik link di atas untuk langsung membuka aplikasi tanpa perlu install apapun!

### Install Lokal (Opsional)

```bash
git clone https://github.com/mahar-debug/Retrolens-Mobile.git
cd Retrolens-Mobile
pip install -r requirements_streamlit.txt
```

### Jalankan di Laptop/Desktop

```bash
streamlit run streamlit_app.py
```

Aplikasi akan terbuka di browser: `http://localhost:8501`

### Akses dari HP (Same WiFi)

1. **Di Laptop**, jalankan command di atas
2. **Lihat IP address** yang muncul di terminal (misal: `192.168.1.100`)
3. **Di HP**, buka browser: `http://192.168.1.100:8501`
4. Tap **"📹 Live Camera"** dan allow akses kamera
5. **Mulai gunakan!**

---

## 🎮 Controls

### Gesture Controls
- **Spread both hands** → Open portal / Create portal area
- **Pinch thumb + pinky** → Switch filter
- **Clench both fists** → Toggle mode 2D/3D

### Button Controls
- **🔄 2D/3D** - Toggle between 2D and 3D mode
- **→ Next** - Switch to next filter
- **Filter Buttons** - Quick select filters from sidebar

### Settings
- **Pinch Sensitivity** - Adjust how sensitive pinch detection is
- **Fist Detection** - Adjust fist clenching sensitivity

---

## 📋 Modes

### Live Camera Mode
- Real-time hand tracking from your camera
- Instant filter application
- Adjustable settings on the fly

### Upload Video Mode
- Process video files with filters
- Watch the progress bar
- See the result in real-time

---

## 🎨 Available Filters

1. **Dual-tone** - Classic two-color effect
2. **Thermal** - Heat map visualization
3. **Sketch** - Pencil drawing effect
4. **Pixelate** - Pixel block effect
5. **Glitch** - Digital glitch distortion
6. **Invert** - Negative film effect
7. **Red-channel** - Red color only
8. **Edge** - Edge detection effect
9. **Blur** - Gaussian blur effect
10. **Cartoon** - Cartoon rendering
11. **Rainbow-wave** - Animated rainbow waves

---

## 🔧 Customization

Edit `PipelineConfig` in `streamlit_app.py`:

```python
@dataclass
class PipelineConfig:
    frame_width: int = 960              # Frame width
    frame_height: int = 540             # Frame height
    pinch_threshold_px: float = 45.0    # Pinch detection threshold
    filter_cooldown_sec: float = 0.15   # Filter switch cooldown
    mode_cooldown_sec: float = 1.2      # Mode toggle cooldown
    fist_dist_threshold_px: float = 80.0  # Fist detection threshold
```

---

## 📦 Requirements

- Python 3.8+
- OpenCV (cv2)
- MediaPipe
- Streamlit
- NumPy

---

## 🎬 Quick Demo

1. **Open the Streamlit Cloud link above**
2. Choose **"📹 Live Camera"**
3. Allow camera access
4. Spread both hands to create portal
5. Pinch thumb + pinky to change filter
6. Enjoy! ✨

---

## 📄 License

MIT License

---

## 👤 Author

- **Developer:** [@mahar-debug](https://github.com/mahar-debug)
- **Built with:** [MediaPipe](https://mediapipe.dev/) and [OpenCV](https://opencv.org/)
- **Powered by:** [Streamlit](https://streamlit.io/)

---

## 💡 Tips

- Make sure you have good lighting for better hand tracking
- Keep your hands within camera view
- Allow camera permissions when prompted
- For best results, use a device camera or phone with good autofocus
- Adjust sensitivity sliders if tracking feels off

---

## 🐛 Troubleshooting

### Camera not detected
- Check if camera permission is granted
- Try allowing camera access in browser settings

### Hand tracking not working
- Ensure good lighting
- Keep hands in clear view
- Adjust detection confidence in settings

### Slow performance
- Reduce frame width/height in settings
- Close other applications
- Check your internet connection

---

## 🚀 Deployment Options

### Option 1: Streamlit Cloud (Recommended - Already Set Up!)
- ✅ **Free hosting**
- ✅ **No configuration needed**
- ✅ **Auto-updates from GitHub**
- Just click the button at the top!

### Option 2: Run Locally
```bash
streamlit run streamlit_app.py
```

---

## 🌐 How It Works

1. **GitHub Repository** contains the code
2. **Streamlit Cloud** automatically deploys from this repo
3. **No servers to manage** - just push to GitHub!
4. **Live updates** - changes appear instantly

---

**Happy filtering!** 🎨✨

---

**GitHub:** https://github.com/mahar-debug/Retrolens-Mobile  
**Live Demo:** https://retrolens-mobile-mahar.streamlit.app
