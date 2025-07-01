# 🎹 Synthwave Piano Simulator 🎶

<p align="center">
  A real-time, synthwave-inspired virtual piano built in <b>C</b> using <b>PortAudio</b> for audio synthesis and <b>SDL2</b> for animated GUI keys. Supports multiple waveforms, quantum-based note switching, delay effects, and a round-robin note scheduling system.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/74038190/229223263-cf2e4b07-2615-4f87-9c38-e37600f8381a.gif" width="80%" alt="Synthwave Piano Demo">
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
![image](https://github.com/user-attachments/assets/a55e4a50-c46a-4764-b1cd-2fa262d84f5c)
![image](https://github.com/user-attachments/assets/34673fdf-782b-454d-9e70-7e0dcbeb2e95)
![image](https://github.com/user-attachments/assets/0d70b70f-944b-438d-a21f-201c746259db)


<p align="center">
  <img src="https://user-images.githubusercontent.com/74038190/229223263-cf2e4b07-2615-4f87-9c38-e37600f8381a.gif" width="80%">
</p>

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

Pull requests and forks are welcome — feel free to extend with your effects, visualizations, or improvements!

---

## 📑 License

This project is released under the **MIT License**.

---

## 🙌 Author

**A.M. Mukilan**  


🔗 [GitHub Profile](https://github.com/MUKILAN0608)

---



---

<p align="center">
  <b>🎵 Happy Coding & Music Making! 🎵</b>
</p>
