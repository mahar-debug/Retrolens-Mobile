# RetroLens Mobile & Desktop 🖐️✨

**Real-time hand tracking portal filter** - Works perfectly on **HP, Tablet, and Laptop!**

Based on the original [syahdanfx/Retrolens](https://github.com/syahdanfx/Retrolens) project, this version uses **Streamlit** for easy mobile & desktop deployment.

---

## 🌟 Features

- ✅ **Live Camera** - Real-time hand gesture tracking
- ✅ **Video Upload** - Process video files with filters
- ✅ **11 Filters** - Dual-tone, Thermal, Sketch, Pixelate, Glitch, Invert, Red-channel, Edge, Blur, Cartoon, Rainbow-wave
- ✅ **2D/3D Mode** - Toggle between different gesture detection modes
- ✅ **Mobile Responsive** - Perfect on HP, Tablet, and Laptop
- ✅ **No Installation Hassle** - Works with simple `pip install`
- ✅ **Real-time Settings** - Adjust sensitivity on-the-fly

---

## 📱 Cara Menggunakan (Indonesian)

### Install

```bash
pip install -r requirements_streamlit.txt
```

> ⚠️ **Pengguna Apple Silicon:** jangan upgrade mediapipe dari versi yang di-pin (`0.10.9`)

### Jalankan di Laptop/Desktop

```bash
streamlit run retrolens_streamlit.py
```

Aplikasi akan terbuka di browser: `http://localhost:8501`

### Akses dari HP (Same WiFi)

1. **Di Laptop**, jalankan command di atas
2. **Lihat IP address** yang muncul di terminal (misal: `192.168.1.100`)
3. **Di HP**, buka browser: `http://192.168.1.100:8501`
4. Tap **"📹 Live Camera"** dan allow akses kamera
5. **Mulai gunakan!**

---

## 🎮 Kontrol

### Gesture Controls
- **Bentangin 2 tangan** → Buka portal / Create portal area
- **Pinch jempol + kelingking** → Ganti filter / Switch filter
- **Kepal 2 tangan** → Toggle mode 2D/3D

### Button Controls
- **🔄 2D/3D** - Toggle between 2D and 3D mode
- **→ Next** - Switch to next filter
- **Filter Buttons** - Quick select filters from sidebar

### Settings
- **Pinch Sensitivity** - Adjust how sensitive pinch detection is
- **Fist Detection** - Adjust fist clenching sensitivity

---

## 🇬🇧 English Guide

### Installation

```bash
pip install -r requirements_streamlit.txt
```

### Run on Desktop/Laptop

```bash
streamlit run retrolens_streamlit.py
```

Browser will open at: `http://localhost:8501`

### Access from Mobile Phone

1. **On Laptop**, run the command above
2. **Find the IP address** shown in terminal (e.g., `192.168.1.100`)
3. **On Phone**, open browser: `http://192.168.1.100:8501`
4. Tap **"📹 Live Camera"** and allow camera access
5. **Start using!**

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

## 🛠️ Customization

Edit `PipelineConfig` in `retrolens_streamlit.py`:

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

## 🎬 Demo

1. Open app
2. Choose "📹 Live Camera"
3. Allow camera access
4. Spread both hands to create portal
5. Pinch thumb + pinky to change filter
6. Enjoy! ✨

---

## 📄 License

MIT License - See original [Retrolens](https://github.com/syahdanfx/Retrolens) for details

---

## 🙏 Credits

- Original project: [syahdanfx/Retrolens](https://github.com/syahdanfx/Retrolens)
- Streamlit adaptation by [@mahar-debug](https://github.com/mahar-debug)
- Built with [MediaPipe](https://mediapipe.dev/) and [OpenCV](https://opencv.org/)

---

## 💡 Tips

- Make sure you have good lighting for better hand tracking
- Keep your hands within camera view
- Allow camera permissions when prompted
- For best results, use a desktop camera or phone with good autofocus
- Adjust sensitivity sliders if tracking feels off

---

## 🐛 Troubleshooting

### Camera not detected
- Check if camera permission is granted
- Try `cam_index=1` or `cam_index=2` for different cameras

### Hand tracking not working
- Ensure good lighting
- Keep hands in clear view
- Adjust detection confidence in settings

### Slow performance
- Reduce frame width/height in settings
- Close other applications
- Check your internet connection (for mobile access)

---

## 🚀 Future Improvements

- [ ] Add more filter effects
- [ ] Gesture recording
- [ ] Filter presets
- [ ] Performance optimization for mobile
- [ ] Multi-hand gestures

---

**Happy filtering!** 🎨✨
