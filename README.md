# 🎹 Synthwave Piano Simulator 🎶

<p align="center">
  A real-time, synthwave-inspired virtual piano built in <b>C</b> using <b>PortAudio</b> for audio synthesis and <b>SDL2</b> for animated GUI keys. Supports multiple waveforms, quantum-based note switching, delay effects, and a round-robin note scheduling system.
</p>


---

## 🎛️ Features  

- 🎼 **36-key virtual piano** (C2 to C7)  
- 🎵 **Selectable waveforms:**
  - Sine  
  - Sawtooth  
  - Square  
  - Triangle  
- 🕒 **Quantum-based round-robin scheduling**  
- 🔂 Optional **delay effect** for reverb-style audio  
- 🚫 **Limiter** to avoid audio clipping  
- 🎹 Animated **SDL2 piano interface**
- 🧵 **Multi-threaded:** Audio + GUI run independently  
- 🖥️ Supports **Linux** and **Windows**

---

## 📦 Dependencies  

### 🐧 Linux  
- `libsdl2-dev`  
- `libportaudio2`, `libportaudiocpp0`, `portaudio19-dev`  
- `gcc`  
- `pthread` (native on Unix)

Install via terminal:
```bash
sudo apt-get update
sudo apt-get install libsdl2-dev portaudio19-dev
```

### 🪟 Windows
- SDL2 Development Libraries
- PortAudio v19
- A C compiler like MinGW-w64 or MSYS2

Add SDL2 and PortAudio include/lib paths to your compiler.

---

## 🔧 Build Instructions

### 🐧 Linux
```bash
gcc -o synthwave_piano synthwave_piano.c -lSDL2 -lportaudio -lpthread -lm
./synthwave_piano
```

### 🪟 Windows (MinGW example)
```bash
gcc -o synthwave_piano.exe synthwave_piano.c -IC:/SDL2/include -LC:/SDL2/lib -lmingw32 -lSDL2main -lSDL2 -lportaudio -lwinmm -lpthread -lm
synthwave_piano.exe
```

⚠️ **Note:** Replace `C:/SDL2/` with your actual SDL2 installation path.

---

## 📑 Usage

**1️⃣** On program launch, you'll be prompted to:
- Enter number of active notes (1-36)
- Enter key numbers (1-36, C2 = 1, C#2 = 2 … C7 = 36)
- Enter quantum time (seconds per note)
- Choose waveform type:
  - `1` → Sine
  - `2` → Sawtooth
  - `3` → Square
  - `4` → Triangle

**2️⃣** The piano GUI window will open — currently playing keys will be highlighted.

**3️⃣** Close the window to stop playback and exit.

---

## 📸 Demo

*Synthwave-style animated piano GUI with real-time sound*

![Console Interface](https://github.com/user-attachments/assets/a55e4a50-c46a-4764-b1cd-2fa262d84f5c)

![Piano GUI](https://github.com/user-attachments/assets/34673fdf-782b-454d-9e70-7e0dcbeb2e95)

![Waveform Selection](https://github.com/user-attachments/assets/0d70b70f-944b-438d-a21f-201c746259db)

---

## 🛠️ Future Plans

- ⌨️ Real-time keyboard key input
- 🖱️ GUI-based note selection
- 🎶 Real-time effect toggles (delay, limiter)
- 📊 Dynamic waveform visualizations
- 🎹 MIDI keyboard input support

---

## 📂 Project Structure

```
.
├── synthwave_piano.c     # Source Code
├── README.md             # Documentation
└── assets/               # (Optional: Screenshots, GIFs)
```

---

## 🚀 Contributing

We welcome contributions to make this synthwave piano even more awesome! Here's how you can contribute:

### 🤝 How to Contribute

1. **Fork the Repository**
   ```bash
   # Click the "Fork" button on GitHub or use GitHub CLI
   gh repo fork MUKILAN0608/synthwave-piano-simulator
   ```

2. **Clone Your Fork**
   ```bash
   git clone https://github.com/MUKILAN0608/synthwave-piano-simulator.git
   cd synthwave-piano-simulator
   ```

3. **Create a Feature Branch**
   ```bash
   git checkout -b feature/your-amazing-feature
   # or
   git checkout -b bugfix/fix-description
   ```

4. **Make Your Changes**
   - Add new features, fix bugs, or improve documentation
   - Test your changes thoroughly on both Linux and Windows
   - Follow the existing code style and structure

5. **Commit Your Changes**
   ```bash
   git add .
   git commit -m "✨ Add amazing new feature: [brief description]"
   ```

6. **Push to Your Fork**
   ```bash
   git push origin feature/your-amazing-feature
   ```

7. **Create a Pull Request**
   - Go to your fork on GitHub
   - Click "New Pull Request"
   - Add a clear title and description of your changes
   - Reference any related issues

### 🎯 Contribution Ideas

- **🎹 New Features:**
  - Real-time keyboard input
  - MIDI controller support
  - Additional waveforms (FM synthesis, noise, etc.)
  - Audio recording/export functionality
  - Preset saving/loading system

- **🎨 UI/UX Improvements:**
  - Enhanced visual effects
  - Customizable themes
  - Responsive GUI scaling
  - Visual waveform display

- **🔧 Technical Enhancements:**
  - Cross-platform compatibility improvements
  - Performance optimizations
  - Better error handling
  - Memory leak fixes

- **📚 Documentation:**
  - Code comments and documentation
  - Tutorial videos or GIFs
  - Installation guides for different systems
  - API documentation

### 📋 Pull Request Guidelines

- **Title Format:** Use descriptive titles with emojis (e.g., "🎵 Add triangle wave synthesis")
- **Description:** Clearly explain what your PR does and why
- **Testing:** Ensure your code compiles and runs on both Linux and Windows
- **Code Style:** Maintain consistent formatting and naming conventions
- **Small Commits:** Keep changes focused and atomic when possible

### 🐛 Bug Reports

Found a bug? Please open an issue with:
- **System Info:** OS, compiler version, library versions
- **Steps to Reproduce:** Clear step-by-step instructions
- **Expected vs Actual:** What should happen vs what actually happens
- **Logs/Screenshots:** Any error messages or visual issues

### 💡 Feature Requests

Have an idea? Open an issue with the `enhancement` label and describe:
- **Use Case:** Why would this feature be useful?
- **Implementation Ideas:** Any thoughts on how it could work?
- **Examples:** Similar features in other software?

---

**Thank you for helping make Synthwave Piano Simulator even better! 🎶**

---

## 📑 License

This project is released under the **MIT License**.

---

## 🙌 Author

**A.M. Mukilan**  
*AI & ML Engineer | Full-Stack Developer | Synthwave Tech Enthusiast*

🔗 [GitHub Profile](https://github.com/MUKILAN0608)

---




<p align="center">
  <b>🎵 Happy Coding & Music Making! 🎵</b>
</p>
