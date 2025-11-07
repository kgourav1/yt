# 🎬 yt-dlp Command Generator

A beautiful, user-friendly web application that generates ready-to-use yt-dlp commands for downloading YouTube videos, playlists, and audio files. Simply paste a YouTube URL and get instant access to 20+ pre-configured download commands!

![YouTube Theme](https://img.shields.io/badge/Theme-YouTube-red?style=for-the-badge&logo=youtube)
![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

## ✨ Features

- 🎨 **YouTube-Themed UI** - Dark theme with YouTube's signature red, black, and white colors
- 📋 **20+ Pre-configured Commands** - Download videos, audio, thumbnails, subtitles, and more
- 🔄 **Dynamic URL Insertion** - Automatically adds your YouTube URL to commands
- 📱 **Fully Responsive** - Works perfectly on desktop, tablet, and mobile devices
- 🎯 **One-Click Copy** - Copy any command to clipboard with a single click
- 📚 **Comprehensive Help Guide** - Complete installation and usage instructions
- ⚡ **No Dependencies** - Pure HTML, CSS, and JavaScript (no frameworks needed)
- 🎭 **Smooth Animations** - Beautiful hover effects and transitions

## 🚀 Quick Start

### Option 1: Direct Use
1. Download the `index.html` file
2. Open it in any modern web browser
3. Paste a YouTube URL and start generating commands!

### Option 2: Local Server
```bash
# Clone or download this repository
git clone https://github.com/yourusername/yt-dlp-command-generator.git

# Navigate to the directory
cd yt-dlp-command-generator

# Open with your default browser
# Or use a local server (optional)
python -m http.server 8000
# Then visit: http://localhost:8000
```

## 📖 How to Use

### Step 1: Access the Generator
Open the `index.html` file in your web browser.

### Step 2: Enter YouTube URL
Paste any YouTube video or playlist URL into the input field.

### Step 3: Generate Commands
Click the "Generate Commands" button or press Enter.

### Step 4: Copy & Use
Click "Copy Command" on any card to copy the command to your clipboard, then paste it into Command Prompt or Terminal.

## 🎯 Available Commands

The generator provides commands for:

| Category | Commands |
|----------|----------|
| **Video Downloads** | Best Quality, MP4 Format, 720p Quality, Playlists |
| **Audio Downloads** | MP3 Conversion, Premium MP3 (with metadata), Audio with Thumbnail |
| **Thumbnails** | Download Only, Convert to JPG |
| **Subtitles** | Download Subtitles, Embed Subtitles |
| **Advanced** | Time Range, Speed Limiting, Date Filters, Info Only |

## 🛠️ Prerequisites

Before using the generated commands, you need:

### 1. Install yt-dlp
**Windows:**
```bash
# Download from GitHub
https://github.com/yt-dlp/yt-dlp/releases

# Or install via pip
pip install yt-dlp
```

**Linux/Mac:**
```bash
# Using pip
pip install yt-dlp

# Or using homebrew (Mac)
brew install yt-dlp
```

### 2. Install FFmpeg (Recommended)
FFmpeg is required for merging video and audio streams.

**Windows:**
- Download from https://ffmpeg.org/download.html
- Add to system PATH

**Linux:**
```bash
sudo apt install ffmpeg  # Ubuntu/Debian
sudo yum install ffmpeg  # CentOS/RHEL
```

**Mac:**
```bash
brew install ffmpeg
```

## 💡 Usage Examples

### Example 1: Download Best Quality Video
```bash
yt-dlp "https://www.youtube.com/watch?v=dQw4w9WgXcQ"
```

### Example 2: Download as MP3
```bash
yt-dlp -x --audio-format mp3 "https://www.youtube.com/watch?v=dQw4w9WgXcQ"
```

### Example 3: Download with Metadata and Thumbnail
```bash
yt-dlp -x --audio-format mp3 --audio-quality 0 --embed-thumbnail --add-metadata -o "%(title)s.%(ext)s" "https://www.youtube.com/watch?v=dQw4w9WgXcQ"
```

### Example 4: Download Entire Playlist
```bash
yt-dlp "https://www.youtube.com/playlist?list=PLxxxxxxxxxxxxxx"
```

## 🎨 Customization

The website uses a YouTube-inspired color scheme:

```css
--background: #181818    /* Dark background */
--card-bg: #212121       /* Card background */
--accent: #FF0000        /* YouTube red */
--text: #ffffff          /* White text */
--text-secondary: #aaa   /* Gray text */
```

You can easily customize colors by editing the CSS variables in the `<style>` section.

## 📁 Project Structure

```
yt-dlp-command-generator/
│
├── index.html          # Main application file (all-in-one)
├── README.md           # This file
└── LICENSE             # License file (optional)
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

### Ideas for Contributions:
- Add more command templates
- Support for additional platforms (beyond YouTube)
- Dark/Light theme toggle
- Command history feature
- Export commands to file
- Batch URL processing

## 🐛 Known Issues

- Copy function may not work on very old browsers (IE11 and below)
- Some advanced yt-dlp features are not yet included

## 🔧 Troubleshooting

### Commands Not Working?

1. **"yt-dlp is not recognized"**
   - Add yt-dlp to your system PATH
   - Or run commands from the folder containing yt-dlp.exe

2. **Video and Audio Not Merging?**
   - Install FFmpeg and add it to PATH
   - Restart Command Prompt after installation

3. **Copy Button Not Working?**
   - Enable clipboard permissions in your browser
   - Try using a modern browser (Chrome, Firefox, Edge)

4. **Downloads Failing?**
   - Update yt-dlp: `yt-dlp -U`
   - Check your internet connection
   - Verify the YouTube URL is valid

## 📚 Resources

- [yt-dlp Official Documentation](https://github.com/yt-dlp/yt-dlp)
- [yt-dlp GitHub Repository](https://github.com/yt-dlp/yt-dlp)
- [FFmpeg Official Website](https://ffmpeg.org/)
- [YouTube Terms of Service](https://www.youtube.com/t/terms)

## ⚖️ Legal Disclaimer

This tool is for educational purposes only. Users are responsible for complying with:
- YouTube's Terms of Service
- Copyright laws in their jurisdiction
- Content creators' rights

**Note:** Downloading copyrighted content without permission may be illegal in your country.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**Kumar Gourav**

- GitHub: [@yourusername](https://github.com/kgourav1)

## 🙏 Acknowledgments

- [yt-dlp](https://github.com/yt-dlp/yt-dlp) - The amazing command-line tool this generator is built for
- [FFmpeg](https://ffmpeg.org/) - For video/audio processing
- YouTube - For the design inspiration

## 📊 Project Stats

- **Size:** ~25KB (single HTML file)
- **Load Time:** < 100ms
- **Browser Support:** All modern browsers
- **Commands Available:** 20+
- **Last Updated:** November 2025

## 🌟 Star History

If you find this project useful, please consider giving it a star ⭐ on GitHub!

---

**Made with ❤️ by Kumar Gourav**

*Remember to use this tool responsibly and respect content creators' rights!*
