VidSnap AI 🎬

A Flask-based web app that transforms your photos and text into Instagram-ready reels with AI-generated voiceovers powered by ElevenLabs.

---

🖼️ Screenshots

Home Page
[Home Page](screenshots/home.png)

Create Reel
[Create Reel](screenshots/create.png)

Reel Gallery
[Gallery](screenshots/gallery.png)

---

✨ Features

- Upload multiple images to generate a reel
- AI-powered voiceover generation using ElevenLabs API
- Video stitching using FFmpeg
- Gallery to view all generated reels
- Simple and clean web interface

---

🛠️ Tech Stack

- **Backend:** Python, Flask
- **Video Processing:** FFmpeg (via subprocess)
- **AI Voiceover:** ElevenLabs API
- **Other:** uuid, python-dotenv

---

⚙️ Setup & Installation

Prerequisites

- Python 3.8+
- FFmpeg installed on your system ([Download here](https://ffmpeg.org/download.html))
- ElevenLabs API key ([Get one here](https://elevenlabs.io))

Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/Avi-choudhary/VidSnap-AI.git
   cd VidSnap-AI
   ```

2. **Install dependencies**
   ```bash
   pip install flask elevenlabs python-dotenv
   ```

3. **Configure API key**

   Copy the example config file and add your ElevenLabs API key:
   ```bash
   cp config_example.py config.py
   ```
   Then open `config.py` and replace the placeholder with your actual API key.

4. **Run the app**
   ```bash
   python main.py
   ```

5. Open your browser and go to `http://localhost:5000`

---

🚀 Usage

1. Go to **Create Reel** from the navbar
2. Upload one or more images
3. Enter the text you want as voiceover
4. Click **Create Reel**
5. View your generated reel in the **Gallery**

---

📁 Project Structure

```
VidSnap-AI/
├── main.py               # Flask app entry point
├── generate_process.py   # Video generation logic
├── text_to_audio.py      # ElevenLabs voiceover generation
├── config_example.py     # Example config (copy to config.py)
├── static/               # CSS, JS, static assets
├── templates/            # HTML templates
└── .gitignore
```

---

⚠️ Note

This project requires your own ElevenLabs API key to generate voiceovers. Free tier tokens are limited — see [ElevenLabs pricing](https://elevenlabs.io/pricing) for details.

---

👨‍💻 Author

**Avi Choudhary**  
B.Tech IIoT, USAR, GGSIPU  
[GitHub](https://github.com/Avi-choudhary)
