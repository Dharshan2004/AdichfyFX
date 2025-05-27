# 🎵 Modular Soundboard

A modern, feature-rich soundboard application born out of necessity for student-organized events. While showcased as a Tamil Dialogue Soundboard, this is a completely modular system that can be tailored to any audio collection or use case.

![Soundboard Preview](https://img.shields.io/badge/Status-Live-brightgreen) ![License](https://img.shields.io/badge/License-MIT-blue) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 🎯 Project Origin

This soundboard was created out of **necessity** for a student-organized event where we needed:
- A **simple, reliable** way to play audio clips during presentations
- **Quick access** to specific sounds via keyboard shortcuts
- **Easy organization** of audio files by categories
- **No complex setup** or dependencies - just open and use
- **Professional appearance** suitable for public events

What started as a quick solution for Tamil movie dialogues evolved into a **modular, customizable soundboard** that can serve any audio collection needs.

## ✨ Features

### 🎮 **Core Functionality**
- **Instant Audio Playback** - Click buttons or use keyboard shortcuts
- **Smart Audio Management** - Single or multi-sound playback modes
- **Real-time Search** - Filter sounds across all categories
- **Volume Control** - Global volume slider with live adjustment
- **Random Play** - Discover sounds with random selection

### 🎨 **Modern UI/UX**
- **Glassmorphism Design** - Beautiful, modern interface
- **Responsive Layout** - Works perfectly on desktop, tablet, and mobile
- **Smooth Animations** - Professional transitions and hover effects
- **Category Organization** - Collapsible sections with color coding
- **Visual Feedback** - Playing sounds show pulse animations

### ⚙️ **Admin Mode (Easy Customization)**
- **Visual Sound Editor** - Edit labels, categories, and shortcuts without touching code
- **Add New Sounds** - Upload and configure new audio files
- **Category Management** - Create custom categories with colors
- **Keyboard Shortcuts** - Assign keys with duplicate detection
- **Backup & Restore** - Export/import configurations
- **Auto-save** - Changes persist in browser storage

### 🔧 **Technical Features**
- **No Dependencies** - Pure HTML, CSS, and JavaScript
- **Offline Ready** - Works with local web server
- **Auto-discovery** - Automatically detects audio files
- **Fallback System** - Graceful handling of missing files
- **Local Storage** - Remembers your customizations

## 🚀 Quick Start

### 1. **Download & Setup**
```bash
# Clone or download the repository
git clone https://github.com/yourusername/modular-soundboard.git
cd modular-soundboard

# Add your audio files to the sounds/ folder
cp your-audio-files.mp3 sounds/
```

### 2. **Start Local Server**
```bash
# Using Python 3
python3 -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000

# Using Node.js (if you have it)
npx http-server

# Using PHP
php -S localhost:8000
```

### 3. **Open in Browser**
Navigate to `http://localhost:8000` and start using your soundboard!

## 🎮 How to Use

### **Basic Usage**

#### **Playing Sounds**
- **Click any sound button** to play that audio clip
- **Use keyboard shortcuts** (1-9, 0, Q, W, E, etc.) for quick access
- **Search for sounds** using the search bar at the top
- **Adjust volume** with the global volume slider

#### **Audio Control**
- **Single Mode** (default): Only one sound plays at a time
- **Multi Mode**: Click the toggle to allow multiple sounds simultaneously
- **Stop All**: Click "Stop All" button to silence everything
- **Random Play**: Click "Random" to play a surprise sound

#### **Organization**
- **Categories**: Sounds are organized into collapsible categories
- **Click category headers** to expand/collapse sections
- **Color coding**: Each category has its own color for easy identification

### **Advanced Features**

#### **Search & Filter**
- Type in the search box to filter sounds in real-time
- Search works across all categories and sound labels
- Clear search to see all sounds again

#### **Keyboard Shortcuts**
- **Number keys (1-0)**: Play assigned sounds
- **Letter keys (Q,W,E,R,T,Y,U,I,O,P)**: Additional sound shortcuts
- **Escape**: Clear search (when search is focused)
- Shortcuts are disabled when typing in search or admin mode

#### **Volume Control**
- **Global volume slider**: Affects all sounds
- **Real-time adjustment**: Changes apply to currently playing sounds
- **Percentage display**: Shows current volume level

### **Admin Mode (Customization)**

#### **Entering Admin Mode**
1. Click the **"⚙️ Admin"** button in the top-right corner
2. The interface switches to edit mode
3. Sound buttons now show edit icons and open edit forms when clicked

#### **Editing Existing Sounds**
1. **In Admin Mode**: Click any sound button or "Edit" in the sound list
2. **Modify properties**:
   - Change the display label
   - Switch to a different category
   - Assign/change keyboard shortcut
3. **Save changes** or cancel to discard
4. **Delete sounds** if no longer needed

#### **Adding New Sounds**
1. **Select audio file**: Choose MP3 or WAV file
2. **Enter label**: Give it a descriptive name
3. **Choose category**: Select from existing categories
4. **Assign shortcut** (optional): Pick an available key
5. **Click "Add Sound"**
6. **Important**: Manually copy the audio file to your `sounds/` folder

#### **Managing Categories**
1. **Create new categories**: Enter name and pick a color
2. **Categories auto-update**: Available in all dropdowns
3. **Color coding**: Each category gets its unique color

#### **Backup & Restore**
1. **Export Configuration**: Download your settings as JSON
2. **Import Configuration**: Upload a previously saved configuration
3. **Auto-save**: Changes are automatically saved to browser storage

### **Tips for Events**

#### **Preparation**
- **Test all sounds** before your event
- **Assign keyboard shortcuts** to frequently used sounds
- **Organize by usage**: Put most-used sounds in easily accessible categories
- **Export configuration** as backup before the event

#### **During Events**
- **Use keyboard shortcuts** for quick access during presentations
- **Single mode** prevents accidental overlapping sounds
- **Volume control** for different venue acoustics
- **Search function** to quickly find specific sounds

#### **Troubleshooting**
- **No sound**: Check if audio files are in the `sounds/` folder
- **Can't load sounds**: Ensure you're using a web server (not file://)
- **Keyboard shortcuts not working**: Make sure search box isn't focused
- **Changes not saving**: Check browser permissions for local storage

## 🎛️ Customization Guide

### **For Tamil Dialogues (Default Setup)**
The soundboard comes pre-configured with Tamil movie dialogues, but you can easily adapt it:

### **For Any Other Use Case**

#### **Option 1: Use Admin Mode (Recommended)**
1. Click the **"⚙️ Admin"** button in the top-right
2. **Add new sounds** with custom labels and categories
3. **Edit existing sounds** to match your needs
4. **Create new categories** (e.g., "Sound Effects", "Music", "Announcements")
5. **Export your configuration** for backup

#### **Option 2: Edit Configuration File**
Modify `sounds.json` to match your needs:

```json
{
  "sounds": {
    "your-audio-file.mp3": {
      "label": "Your Custom Label",
      "category": "Your Category",
      "key": "1"
    }
  },
  "categories": {
    "Your Category": "#ff6b6b",
    "Another Category": "#4ecdc4"
  }
}
```

### **Common Use Cases**

#### 🎭 **Theater/Drama Productions**
- **Categories**: "Act 1", "Act 2", "Sound Effects", "Music"
- **Sounds**: Scene transitions, background music, sound effects
- **Shortcuts**: Quick access during live performances

#### 🎮 **Gaming/Streaming**
- **Categories**: "Reactions", "Memes", "Alerts", "Music"
- **Sounds**: Subscriber alerts, funny reactions, background music
- **Shortcuts**: Instant reactions during streams

#### 🏫 **Educational Events**
- **Categories**: "Introductions", "Transitions", "Applause", "Background"
- **Sounds**: Event music, transition sounds, applause tracks
- **Shortcuts**: Smooth event flow management

#### 🎉 **Parties/Events**
- **Categories**: "Dance", "Games", "Announcements", "Ambient"
- **Sounds**: Party music, game sounds, announcement chimes
- **Shortcuts**: DJ-style quick mixing

#### 📻 **Podcast/Radio**
- **Categories**: "Intros", "Outros", "Transitions", "Effects"
- **Sounds**: Show intros, commercial breaks, transition music
- **Shortcuts**: Professional broadcast control

## 🎹 Keyboard Shortcuts

| Key | Default Sound | Customizable |
|-----|---------------|--------------|
| `1-0` | Tamil Dialogues | ✅ Yes |
| `Q,W,E,R,T,Y,U,I,O,P` | Available for assignment | ✅ Yes |
| `Space` | Stop all sounds | ❌ Fixed |
| `/` | Focus search | ❌ Fixed |

## 📁 File Structure

```
modular-soundboard/
├── index.html          # Main application
├── sounds.json         # Sound configuration
├── sounds/             # Audio files directory
│   ├── your-audio.mp3
│   └── another-sound.wav
└── README.md          # This file
```

## 🔧 Technical Requirements

- **Web Server** (required for file loading)
- **Modern Browser** (Chrome, Firefox, Safari, Edge)
- **Audio Files** in MP3 or WAV format
- **No additional dependencies**

## 🎨 Customization Options

### **Visual Themes**
- Modify CSS variables for colors
- Change gradient backgrounds
- Adjust glassmorphism effects
- Custom category colors

### **Functionality**
- Add new keyboard shortcuts
- Modify audio loading behavior
- Extend admin panel features
- Add new sound categories

### **Integration**
- Embed in existing websites
- Connect to external APIs
- Add database storage
- Implement user accounts

## 🤝 Contributing

This project welcomes contributions! Whether you're:
- Adding new features
- Improving the UI/UX
- Fixing bugs
- Adding documentation
- Sharing use cases

Feel free to open issues or submit pull requests.

## 📄 License

MIT License - feel free to use this project for any purpose, including commercial applications.

## 🙏 Acknowledgments

- Born out of necessity for student event management
- Inspired by modern SaaS application design
- Built with accessibility and ease-of-use in mind
- Community-driven feature requests and improvements

## 📞 Support

If you're using this soundboard for your events or projects, we'd love to hear about it! Share your use cases, customizations, or feedback.

---

**Made with ❤️ for the community** | **Simple, Powerful, Customizable** 