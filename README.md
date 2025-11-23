# 🎙️ VoiceOver

A beautiful, mobile-first Progressive Web App (PWA) for creating voice notes using speech recognition. Built as a single HTML file for maximum portability and ease of deployment.

![VoiceOver App](https://img.shields.io/badge/PWA-Ready-success?style=for-the-badge)
![iOS Compatible](https://img.shields.io/badge/iOS-Safari-blue?style=for-the-badge)
![No Backend Required](https://img.shields.io/badge/Backend-None-green?style=for-the-badge)

## ✨ Features

### 🎤 **Voice Recording**
- Real-time speech-to-text transcription
- Continuous recording with live preview
- iOS Safari compatible (uses `webkitSpeechRecognition`)
- Microphone permission handling with user-friendly error messages

### 📝 **Note Management**
- **Create** new voice notes with a single tap
- **View** full note content in detail view
- **Append** additional content to existing notes
- **Reorder** notes using up/down arrows
- **Delete** notes with confirmation dialog
- **Persist** all notes locally using localStorage

### 🎨 **Beautiful Design**
- Dark theme with purple/indigo gradients
- Smooth fade-in animations
- Pulse effect during recording
- Responsive mobile-first layout
- Native app feel with disabled text selection on UI elements
- Custom scrollbars and hover effects

### 📱 **PWA Capabilities**
- Full-screen mode on iOS (no Safari URL bar)
- "Add to Home Screen" support
- Works offline after initial load
- Native app-like experience

## 🚀 Quick Start

### Option 1: Direct File Access
1. Download `index.html`
2. Open it in Safari (iOS) or Chrome (Desktop)
3. On iOS: Tap Share → "Add to Home Screen"

### Option 2: Local Server
```bash
# Clone the repository
git clone https://github.com/light-saber/voiceover.git
cd voiceover

# Start a local server
python3 -m http.server 8080

# Or use Node.js
npx serve

# Or use PHP
php -S localhost:8080
```

Then open `http://localhost:8080` in your browser.

## 📱 iOS Installation

1. Open the app in **Safari** on your iPhone
2. Tap the **Share** button (square with arrow)
3. Scroll down and tap **"Add to Home Screen"**
4. Name it "VoiceOver" and tap **Add**
5. Launch from your home screen for a full-screen experience!

## 🎯 How to Use

### Creating a New Note
1. Tap the red **microphone button** at the bottom
2. Allow microphone access when prompted
3. Start speaking - your words will appear in real-time
4. Tap **"Save Note"** when finished

### Viewing & Editing Notes
1. Tap any note card to view full content
2. Use the **up/down arrows** to reorder notes
3. Tap the **trash icon** to delete a note
4. Tap **"Append to Note"** to add more content via voice

### Managing Your Notes
- Notes are automatically saved to your device
- Most recent notes appear at the top
- Timestamps show relative time (e.g., "2 hours ago")
- All data persists across app restarts

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **HTML5** | Structure and semantic markup |
| **Tailwind CSS** | Utility-first styling (via CDN) |
| **Vanilla JavaScript** | Logic and interactivity |
| **Web Speech API** | Speech recognition (`webkitSpeechRecognition`) |
| **localStorage** | Client-side data persistence |
| **PWA Meta Tags** | iOS full-screen support |

## 📂 Project Structure

```
voiceover/
├── index.html          # Complete single-file application
└── README.md          # This file
```

Yes, it's really just one file! 🎉

## 🌐 Browser Compatibility

| Browser | Support | Notes |
|---------|---------|-------|
| **Safari (iOS)** | ✅ Full | Recommended for best mobile experience |
| **Chrome (Desktop)** | ✅ Full | Uses standard SpeechRecognition API |
| **Chrome (Android)** | ✅ Full | Full speech recognition support |
| **Firefox** | ⚠️ Limited | Speech recognition not supported |
| **Edge** | ✅ Full | Chromium-based, full support |

## 🔒 Privacy & Security

- **100% Client-Side**: All data stays on your device
- **No Backend**: No server, no database, no tracking
- **No Analytics**: Your notes are completely private
- **localStorage Only**: Data never leaves your browser
- **No External Dependencies**: Except Tailwind CSS CDN

## 🎨 Customization

### Change Color Scheme
Edit the gradient classes in `index.html`:
```html
<!-- Header gradient -->
<header class="bg-gradient-to-r from-purple-600 to-indigo-600">

<!-- Record button -->
<button class="bg-gradient-to-r from-red-500 to-pink-500">
```

### Change Language
Modify the recognition language:
```javascript
recognition.lang = 'en-US'; // Change to 'es-ES', 'fr-FR', etc.
```

### Adjust Recording Behavior
```javascript
recognition.continuous = true;      // Keep listening
recognition.interimResults = true;  // Show real-time results
```

## 🐛 Troubleshooting

### Microphone Not Working
- Ensure microphone permissions are enabled in browser settings
- On iOS, check Settings → Safari → Microphone
- Try reloading the page and granting permission again

### Speech Recognition Not Available
- Use Safari on iOS or Chrome on desktop/Android
- Firefox does not support Web Speech API
- Ensure you're using HTTPS (or localhost for testing)

### Notes Not Saving
- Check if localStorage is enabled in your browser
- Ensure you're not in Private/Incognito mode
- Check browser storage quota (unlikely to be an issue)

### App Not Full-Screen on iOS
- Make sure you added it via "Add to Home Screen"
- Launch from the home screen icon, not Safari
- Check that PWA meta tags are present in the HTML

## 📝 License

MIT License - feel free to use this project for personal or commercial purposes.

## 🤝 Contributing

Contributions are welcome! Here are some ideas:

- [ ] Add support for multiple languages
- [ ] Implement note search/filter functionality
- [ ] Add export notes as text/PDF
- [ ] Implement note categories/tags
- [ ] Add dark/light theme toggle
- [ ] Support for audio playback of notes
- [ ] Cloud sync option (Firebase, etc.)

## 💡 Inspiration

Built for anyone who wants to quickly capture thoughts, ideas, meeting notes, or reminders using their voice. Perfect for:

- 📚 Students taking lecture notes
- 💼 Professionals capturing meeting action items
- ✍️ Writers brainstorming ideas
- 🧠 Anyone who thinks faster than they type

## 🙏 Acknowledgments

- Built with [Tailwind CSS](https://tailwindcss.com/)
- Icons from [Heroicons](https://heroicons.com/)
- Uses the [Web Speech API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API)

## 📧 Contact

Have questions or suggestions? Feel free to open an issue or reach out!

---

**Made with ❤️ for voice note enthusiasts**

⭐ Star this repo if you find it useful!
