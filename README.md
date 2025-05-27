# 🎧 AdichfyFX

A quirky Tamil DJ-style soundboard web app inspired by professional DJ sound pads. Drop the beat with iconic Tamil dialogues (comedy, mass, romantic, reactions) perfect for live events, meme creation, and entertainment. While focused on Tamil cinema sounds, AdichfyFX is a completely modular system that anyone can tailor for their own audio collection.

![Soundboard Preview](https://img.shields.io/badge/Status-Live-brightgreen) ![License](https://img.shields.io/badge/License-MIT-blue) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 🎯 Project Origin

**AdichfyFX** was born out of **necessity** for a student-organized event where we needed:
- A **DJ-style interface** to drop Tamil dialogue beats during live events
- **Instant access** to iconic Tamil cinema moments via keyboard shortcuts
- **Meme-ready sounds** organized by mood and genre (comedy, mass, romantic, reactions)
- **Zero setup complexity** - just open and start dropping beats
- **Professional DJ aesthetics** suitable for public entertainment

What started as a quick solution for Tamil movie dialogue drops evolved into **AdichfyFX** - a modular, customizable soundboard that can serve any audio collection needs while maintaining that signature Tamil cinema vibe.

## ✨ Features

### 🎮 **DJ-Style Core Features**
- **Instant Beat Drops** - Click pads or use DJ-style keyboard shortcuts
- **Smart Audio Mixing** - Single or multi-sound layering modes
- **Live Sound Search** - Filter beats across all categories in real-time
- **Master Volume Control** - Global volume slider with live adjustment
- **Random Beat Discovery** - Surprise yourself with random Tamil gems

### 🎨 **Professional DJ Interface**
- **Glassmorphism Design** - Sleek, modern DJ console aesthetics
- **Responsive Layout** - Perfect for laptop DJs, tablet controllers, and mobile use
- **Smooth Beat Transitions** - Professional animations and hover effects
- **Genre Organization** - Collapsible sections with mood-based color coding
- **Live Visual Feedback** - Playing beats show pulsing DJ-style animations

### ⚙️ **DJ Booth Management (Easy Customization)**
- **Visual Beat Editor** - Edit labels, genres, and shortcuts without touching code
- **Add New Beats** - Upload and configure new Tamil dialogue drops
- **Genre Management** - Create custom mood categories with colors
- **DJ Hotkeys** - Assign any key combination with duplicate detection
- **Set Backup & Restore** - Export/import your DJ configurations
- **Auto-save** - Your DJ setup persists in browser storage

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
git clone https://github.com/yourusername/adichfyfx.git
cd adichfyfx

# Add your Tamil dialogue beats to the sounds/ folder
cp your-tamil-dialogues.mp3 sounds/
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
Navigate to `http://localhost:8000` and start dropping those Tamil beats!

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

### **For Tamil Cinema Beats (Default Setup)**
AdichfyFX comes pre-loaded with iconic Tamil movie dialogues organized by mood, but you can easily customize it:

### **For Any Other Use Case**

#### **Option 1: Use DJ Booth Mode (Recommended)**
1. Click the **"⚙️ Admin"** button to enter DJ Booth management
2. **Add new beats** with custom labels and genres
3. **Edit existing dialogues** to match your vibe
4. **Create new genres** (e.g., "Kuthu Beats", "Emotional", "Troll Sounds")
5. **Export your DJ set** for backup and sharing

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

#### 🎬 **Tamil Cinema Events**
- **Genres**: "Mass Dialogues", "Comedy Punches", "Romantic Lines", "Villain Entries"
- **Beats**: Iconic movie moments, hero introductions, comedy timing
- **Shortcuts**: Instant crowd reactions during live events

#### 🎮 **Meme Creation & Streaming**
- **Genres**: "Troll Sounds", "Reaction Beats", "Viral Dialogues", "Kuthu Drops"
- **Beats**: Perfect for content creation, live streaming reactions
- **Shortcuts**: Instant meme drops during streams

#### 🎉 **College/Cultural Events**
- **Genres**: "Opening Beats", "Transition Sounds", "Applause Tracks", "Closing"
- **Beats**: Event management, crowd engagement, cultural programs
- **Shortcuts**: Smooth event flow with Tamil cinema flavor

#### 🎧 **DJ Sets & Parties**
- **Genres**: "Dance Beats", "Hype Dialogues", "Crowd Pumpers", "Chill Vibes"
- **Beats**: Party mixing, crowd interaction, dance floor energy
- **Shortcuts**: Professional DJ-style quick drops

#### 📻 **Tamil Podcast/Radio**
- **Genres**: "Show Intros", "Segment Transitions", "Comedy Breaks", "Outros"
- **Beats**: Tamil content creation, radio shows, podcast production
- **Shortcuts**: Professional broadcast control with Tamil touch

## 🎹 Keyboard Shortcuts

| Key/Combination | Default Beat | Customizable |
|-----------------|---------------|--------------|
| `1-0` | Iconic Tamil Dialogues | ✅ Yes |
| `Q,W,E,R,T,Y,U,I,O,P` | Available for custom beats | ✅ Yes |
| `Ctrl+[Key]` | Custom combinations | ✅ Yes |
| `Alt+[Key]` | Custom combinations | ✅ Yes |
| `Shift+[Key]` | Custom combinations | ✅ Yes |
| `F1-F12` | Function keys | ✅ Yes |
| `Arrow Keys` | Navigation keys | ✅ Yes |
| `Space`, `Enter`, etc. | Special keys | ✅ Yes |

**Note**: You can now assign any key combination including modifiers (Ctrl, Alt, Shift) and special keys!

## 📁 File Structure

```
adichfyfx/
├── index.html          # Main DJ application
├── sounds.json         # Beat configuration
├── sounds/             # Tamil dialogue beats directory
│   ├── mass-dialogue.mp3
│   ├── comedy-punch.mp3
│   └── romantic-line.wav
├── LICENSE            # MIT License
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

### **Possible Integration**
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

- Born out of necessity for Tamil student event entertainment
- Inspired by professional DJ equipment and Tamil cinema culture
- Built with accessibility and Tamil community in mind
- Community-driven feature requests and Tamil dialogue suggestions

## 📞 Support

If you're using **AdichfyFX** for your events, memes, or DJ sets, we'd love to hear about it! Share your Tamil beat drops, customizations, or feedback.

---

**Made with ❤️ for Tamil cinema lovers** | **Adichfy Your Moments** | **DJ-Style, Tamil-Powered** 
