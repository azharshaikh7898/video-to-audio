# Video-to-Audio Converter 🎬➡️🎵

A simple Python-based tool to convert video files (e.g. MP4, AVI, MKV) into audio formats (MP3, WAV, AAC). Built with an easy‑to‑use UI and batch conversion support.

---

## 🚀 Features

- Convert videos into audio formats: MP3, WAV, AAC
- Customizable bitrate (e.g. 64–320 kbps)
- Batch conversion support
- Progress feedback during conversion
- Optional GUI (e.g. PyQt5 or CLI)
- Choose output directory for extracted audio
- Handles common video input formats

---

## 🛠️ Built With

- **Python 3.6+**
- [MoviePy](https://zulko.github.io/moviepy/) for media processing
- GUI (optional): PyQt5 or CLI script
- Optional: ffmpeg dependency for backend processing

---

## 📁 Repository Structure

├── app.py or main.py # Main script or GUI entry point
├── requirements.txt # Required Python dependencies
├── videos/ # Sample video files (optional)
├── output_audio/ # Default output directory
└── README.md                       

---

## 🔧 Installation

1. Clone the repository:

   
   git clone https://github.com/azharshaikh7898/video-to-audio.git
   cd video-to-audio


   (Optional) Create and activate virtual environment:


python -m venv venv
source venv/bin/activate    # Windows: venv\Scripts\activate
Install dependencies:


pip install -r requirements.txt
(Optional) Install system dependency:


sudo apt install ffmpeg  # macOS/Homebrew: brew install ffmpeg
🎛️ Usage
GUI version (if available):
Run the GUI script:

python app.py
In the interface:

Select one or more video files

Choose output format (MP3/WAV/AAC)

Set bitrate and output directory

Click Convert and observe progress

CLI version (if no GUI):

python main.py --input video1.mp4 video2.mkv --output-dir ./output --format mp3 --bitrate 192
Options (example syntax):

--input or -i: one or more video file paths

--output-dir or -o: output directory (default: output_audio/)

--format or -f: audio format (mp3, wav, aac)

--bitrate or -b: audio bitrate (e.g. 64, 128, …)

✅ Example

python main.py -i sample1.mp4 sample2.mkv -o ./audio_files -f mp3 -b 256
This will convert two video files into MP3 audio at 256 kbps, saving them in ./audio_files/.

🎯 Contributing
Contributions are welcome! Please:

Fork the repository

Create a new branch (feature/my-feature)

Make your changes, commit (git commit -m "Add feature")

Push to your branch and open a Pull Request


