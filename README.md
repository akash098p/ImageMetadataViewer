# 📸 Image Metadata Viewer

A powerful, privacy-focused web application to view and remove EXIF metadata from images. Works 100% offline in your browser - no server uploads required!

## ✨ Features

- **📤 Upload Images** - Drag & drop or click to browse
- **🔍 View All EXIF Data** - Camera, GPS, dates, and more
- **📷 Camera Information** - Make, model, lens, ISO, aperture, shutter speed, focal length
- **🌍 GPS Location** - View coordinates and location on Google Maps
- **🕐 Date & Time** - Capture time, modification time, timezone
- **🗑️ Remove Metadata** - Strip all EXIF data and download clean images
- **🔒 Privacy First** - All processing happens locally in your browser
- **📱 Responsive Design** - Works on desktop, tablet, and mobile
- **⚡ Works Offline** - Once loaded, works without internet connection

## 🚀 Live Demo

Visit the live demo: [https://yourusername.github.io/image-metadata-viewer](https://yourusername.github.io/image-metadata-viewer)

## 📋 What Metadata Can You View?

### Camera & Settings
- Camera make and model
- Lens information
- ISO speed
- Aperture (f-stop)
- Shutter speed
- Focal length
- Exposure program
- Metering mode
- Flash status
- White balance
- Exposure bias

### Location Data
- GPS coordinates (latitude/longitude)
- Altitude
- GPS timestamp
- Direct link to Google Maps

### Date & Time
- Original capture date/time
- Modification date/time
- Digitization date/time
- Timezone information

### Additional Information
- Software used
- Artist/Author
- Copyright information
- Color space
- Image orientation
- Resolution (DPI)
- Image description
- User comments

## 🛠️ Technologies Used

- **HTML5** - Structure and layout
- **CSS3** - Styling with gradients and animations
- **Vanilla JavaScript** - Core functionality
- **EXIF.js** - EXIF metadata extraction library
- **Service Worker** - Offline functionality
- **Canvas API** - Metadata removal

## 📦 Installation & Setup

### Option 1: Deploy to GitHub Pages (Recommended)

1. **Fork or Clone this Repository**
   ```bash
   git clone https://github.com/yourusername/image-metadata-viewer.git
   cd image-metadata-viewer
   ```

2. **Push to Your GitHub Account**
   ```bash
   git remote set-url origin https://github.com/YOUR-USERNAME/image-metadata-viewer.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click on **Settings**
   - Scroll down to **Pages** section
   - Under **Source**, select **main** branch
   - Click **Save**
   - Your site will be published at `https://YOUR-USERNAME.github.io/image-metadata-viewer`

4. **Update Links** (Optional)
   - Edit `index.html` and update the GitHub link in the footer
   - Update the demo link in this README

### Option 2: Run Locally

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/image-metadata-viewer.git
   cd image-metadata-viewer
   ```

2. **Serve the Files**
   
   Using Python:
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Python 2
   python -m SimpleHTTPServer 8000
   ```
   
   Using Node.js:
   ```bash
   npx http-server
   ```
   
   Using VS Code:
   - Install "Live Server" extension
   - Right-click on `index.html`
   - Select "Open with Live Server"

3. **Open in Browser**
   - Navigate to `http://localhost:8000`

## 📁 File Structure

```
image-metadata-viewer/
│
├── index.html          # Main HTML file
├── styles.css          # CSS styling
├── script.js           # JavaScript functionality
├── sw.js              # Service Worker for offline support
└── README.md          # This file
```

## 🔒 Privacy & Security

- **No Server Uploads** - All image processing happens in your browser
- **No Data Storage** - Images are not stored anywhere
- **No Tracking** - No analytics or tracking scripts
- **Open Source** - Fully transparent code you can inspect
- **Offline Capable** - Works without internet after first load

## 🎯 Use Cases

- **Privacy Protection** - Remove location data before sharing photos
- **Photography Analysis** - Study camera settings of professional photos
- **Forensics** - Verify image authenticity and origin
- **Education** - Learn about camera settings and photography
- **Metadata Research** - Analyze EXIF data patterns

## 🌐 Browser Support

Works on all modern browsers that support:
- File API
- Canvas API
- Service Workers (for offline functionality)

Tested on:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🐛 Known Limitations

- Some image formats (like HEIC on certain browsers) may have limited support
- Very large images (>10MB) may take longer to process
- GPS data requires the image to have been taken with location services enabled

## 💡 Tips

- **For Best Results**: Use original, unedited photos directly from your camera or smartphone
- **Privacy**: Always remove metadata before sharing personal photos online
- **Backup**: Keep original files before removing metadata
- **Formats**: JPEG files typically contain the most EXIF data

## 🔮 Future Enhancements

- [ ] Batch processing multiple images
- [ ] Export metadata to JSON/CSV
- [ ] Edit specific metadata fields
- [ ] Compare metadata between images
- [ ] Dark mode theme
- [ ] Additional image formats support
- [ ] Metadata statistics and visualization

## 📧 Contact

For questions, suggestions, or issues:
- Open an issue on GitHub
- Contact: your.email@example.com

## 🙏 Acknowledgments

- [EXIF.js](https://github.com/exif-js/exif-js) - For EXIF data extraction
- Icons - Emoji characters
- Inspired by the need for privacy-focused image tools

---

**Made with ❤️ for privacy-conscious photographers and image enthusiasts**

⭐ If you find this tool useful, please consider giving it a star on GitHub!