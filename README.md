# Drago's Calendar 📅

A minimal, aesthetic desktop calendar widget built with Electron. Features a beautiful purple pixel-art themed design that sits elegantly on your desktop.


## ✨ Features

- **Always-on-top widget**: Stays visible on your desktop
- **Frameless & transparent**: Clean, modern aesthetic with no window chrome
- **Draggable**: Position anywhere on your screen
- **Auto-updating**: Displays current day and month
- **Pixel-art design**: Retro gaming aesthetic with custom purple theme
- **Lightweight**: Minimal resource usage

## 🎨 Design

The app features a custom pixel-art design with:
- Outer frame with pink gradient background
- Inner calendar frame with purple tones
- Pixeboy font for retro gaming vibes
- Smooth transparency and rounded corners

## 📋 Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- npm (comes with Node.js)

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/dragos-calendar.git
   cd dragos-calendar
   ```

2. **Install dependencies**
   ```bash
   npm install electron --save-dev
   ```

3. **Run the app**
   ```bash
   npm start
   ```

## 📁 Project Structure

```
dragos-calendar/
├── assets/
│   ├── inner-frame-bg.png    # Inner calendar frame background
│   └── outer-frame-bg.png    # Outer app frame background
├── index.html                # Main HTML structure
├── styles.css                # Styling and layout
├── script.js                 # Calendar logic
├── main.js                   # Electron main process
├── package.json              # Project dependencies
├── package-lock.json         # Dependency lock file
└── README.md                 # This file
```

## 🛠️ Configuration

### Window Size
The app opens at 214x228 pixels. To change this, edit `main.js`:

```javascript
const win = new BrowserWindow({
  width: 214,  // Change width here
  height: 228, // Change height here
  // ...
});
```

### Styling
All visual customization can be done in `styles.css`:
- Colors: Search for color values like `#C079FF`, `#B58CD9`
- Font sizes: Modify values in the `#day` and `#month` selectors
- Spacing: Adjust `gap`, `padding`, and margin values

## 🎯 Usage

1. Launch the app with `npm start`
2. The calendar widget will appear on your screen
3. Click and drag anywhere on the widget to reposition it
4. The date updates automatically
5. Close by clicking the X (if you add one) or use Task Manager/Activity Monitor
## 🔧 Building for Distribution

To package the app for distribution:

1. **Install electron-builder**
   ```bash
   npm install electron-builder --save-dev
   ```

2. **Add build configuration to package.json**
   ```json
   "build": {
     "appId": "com.drago.calendar",
     "mac": {
       "category": "public.app-category.productivity"
     },
     "win": {
       "target": "nsis"
     },
     "linux": {
       "target": "AppImage"
     }
   },
   "scripts": {
     "start": "electron .",
     "build": "electron-builder"
   }
   ```

3. **Build**
   ```bash
   npm run build
   ```

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests

## 📝 To-Do

- [ ] Fix "February" spelling
- [ ] Add font embedding for Pixeboy
- [ ] Add close/minimize buttons
- [ ] Add settings panel
- [ ] Add multiple theme options
- [ ] Add customizable user name
- [ ] Add day of week display

## 🍿 Preview

<img width="218" height="230" alt="image" src="https://github.com/user-attachments/assets/f284c214-a75b-4aaf-a629-876ca1d13473" />


Made with 💜 by Drago
