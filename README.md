# 📸 Image Metadata Viewer

A fast, professional, and privacy-focused web application to view and remove EXIF metadata from images. Processes metadata in under 1 second with a modern, clean interface.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-2.0.0-green.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

## ✨ Features

### 🚀 Lightning Fast Performance
- **Sub-second processing** - Most images analyzed in <1 second
- Real-time processing timer displayed
- Instant preview and metadata extraction
- Optimized for large images (up to 50MB+)

### 📊 Comprehensive Metadata Reading
- **Camera Information** - Make, model, lens details
- **Camera Settings** - ISO, aperture, shutter speed, focal length
- **GPS Location** - Latitude, longitude, altitude with Google Maps integration
- **Date & Time** - Original, modified, digitized timestamps
- **All EXIF Data** - Complete list of every available metadata field
- **Field Counters** - See exactly how many metadata fields are available

### 🔒 Privacy & Security
- **100% Local Processing** - No server uploads, ever
- **No Data Collection** - Your images never leave your browser
- **Offline Capable** - Works without internet after first load
- **Open Source** - Fully transparent code you can inspect

### 🎨 Professional UI Design
- Modern blue gradient theme
- Clean card-based layout
- Responsive design for all devices
- Smooth animations and transitions
- Intuitive drag-and-drop interface

### 🛠️ Core Functionality
- **Upload Images** - Drag & drop or click to browse
- **View Metadata** - Organized into categories
- **GPS Mapping** - Direct link to location on Google Maps
- **Download Original** - Keep your original file
- **Remove Metadata** - Strip all EXIF data
- **Download Clean** - Get metadata-free version

## 💻 Live Preview 

🔗  https://akash098p.github.io/ImageMetadataViewer/

## 🎯 Supported Formats

- ✅ JPEG / JPG
- ✅ PNG
- ✅ WebP
- ✅ TIFF
- ✅ HEIC (browser dependent)

## 🚀 Quick Start

### Option 1: Open Locally (Easiest)

1. Download all three files:
   - `index.html`
   - `styles.css`
   - `script.js`

2. Place them in the same folder

3. Double-click `index.html` or open it in your browser

4. Start uploading images!

### Option 2: Use a Local Server

If you need to test with a server:

**Using Python:**
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

**Using Node.js:**
```bash
npx http-server
```

**Using PHP:**
```bash
php -S localhost:8000
```

Then open: `http://localhost:8000`

## 🌐 Deploy to GitHub Pages

### Step 1: Create Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click **New Repository**
3. Name it: `image-metadata-viewer`
4. Make it **Public**
5. Click **Create repository**

### Step 2: Upload Files

**Using Git:**
```bash
# Navigate to your project folder
cd ImageMetadataViewer 

# Initialize git
git init

# Add all files
git add index.html styles.css script.js README.md

# Commit
git commit -m "Initial commit: Image Metadata Viewer"

# Add remote (replace YOUR-USERNAME)
git remote add origin https://github.com/YOUR-USERNAME/image-metadata-viewer.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Using GitHub Website:**
1. In your repository, click **Upload files**
2. Drag and drop all files
3. Click **Commit changes**

### Step 3: Enable GitHub Pages

1. Go to repository **Settings**
2. Click **Pages** in the left sidebar
3. Under **Source**, select **main** branch
4. Click **Save**

Your site will be live at:
```
https://akash098p.github.io/ImageMetadataViewer/
```

Wait 1-2 minutes for deployment to complete.

## 📖 How to Use

### Basic Workflow

1. **Upload Image**
   - Drag and drop your image onto the upload area
   - Or click to browse and select a file

2. **View Metadata**
   - Camera settings appear instantly
   - Browse organized categories
   - See processing time

3. **Check Location** (if available)
   - GPS coordinates displayed
   - Click to view on Google Maps

4. **Download Options**
   - Download original with metadata
   - Remove all metadata and download clean version

### Understanding the Interface

**Quick Actions Bar:**
- 🔄 **New Image** - Upload a different image
- ⬇️ **Download Original** - Save the original file
- 🗑️ **Remove Metadata** - Strip EXIF and download

**Left Column:**
- Image preview with zoom
- Basic file information
- GPS location (if available)

**Right Column:**
- Camera & settings details
- Date & time information
- Complete EXIF metadata list

## 🔍 What Metadata Can You See?

### Camera Information
- Camera make and model
- Lens make and model
- ISO speed rating
- Aperture (f-number)
- Shutter speed
- Focal length
- Exposure program/mode
- Metering mode
- Flash status
- White balance
- Exposure compensation

### GPS Data
- Latitude coordinates
- Longitude coordinates
- Altitude (if available)
- GPS timestamp
- Direct Google Maps link

### Date & Time
- Date taken (original)
- Date modified
- Date digitized
- Timezone offset
- Subsecond precision

### Additional Metadata
- Software used
- Artist/Creator
- Copyright information
- Color space
- Resolution (DPI)
- Image orientation
- Image description
- User comments
- And much more...

## 🛠️ Technical Details

### Built With
- **HTML5** - Structure and semantics
- **CSS3** - Modern styling with CSS Grid and Flexbox
- **Vanilla JavaScript** - Zero dependencies for core functionality
- **ExifReader v4.14.0** - Fast and reliable EXIF extraction

### Browser Compatibility
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### Performance
- Average processing time: **0.3 - 0.8 seconds**
- Handles images up to 50MB+
- Memory efficient processing
- Async/await for smooth UX

## 📁 File Structure

```
image-metadata-viewer/
│
├── index.html          # Main HTML structure
├── styles.css          # Professional styling
├── script.js           # Core functionality
└── README.md          # This file
```

## 🎨 Customization

### Change Color Scheme

Edit `styles.css` root variables:

```css
:root {
    --primary: #2563eb;        /* Main blue */
    --primary-dark: #1d4ed8;   /* Darker blue */
    --secondary: #7c3aed;      /* Purple accent */
    --success: #10b981;        /* Green for success */
    --danger: #ef4444;         /* Red for warnings */
}
```

### Modify Processing Limits

Edit `script.js`:

```javascript
// Maximum file size (default: no limit)
const MAX_FILE_SIZE = 50 * 1024 * 1024; // 50MB

// Supported formats
const SUPPORTED_FORMATS = ['image/jpeg', 'image/png', 'image/webp'];
```

## 🔐 Privacy & Security

### Your Data is Safe
- **No Server Communication** - Everything runs in your browser
- **No Cookies** - We don't store anything
- **No Tracking** - Zero analytics or monitoring
- **No Third-Party APIs** - Except optional Google Maps links

### How It Works
1. You upload an image (stays in browser memory)
2. JavaScript reads the EXIF data locally
3. Metadata is displayed on your screen
4. When you close the page, everything is deleted

## 🐛 Troubleshooting

### No Metadata Showing
- Some images (especially from social media) have metadata stripped
- PNG images often don't contain EXIF data
- Try with a photo directly from a camera or smartphone

### Image Won't Upload
- Check file format (must be image/*)
- Ensure file isn't corrupted
- Try a different browser
- Check browser console for errors

### Slow Processing
- Very large images (>20MB) may take 2-3 seconds
- Close other browser tabs to free memory
- Try a different browser

### GPS Not Showing
- Photo must be taken with location services enabled
- Some apps strip GPS data for privacy
- Check "All EXIF Metadata" section for GPSLatitude field

## 🚀 Future Enhancements

Planned features:
- [ ] Batch processing (multiple images)
- [ ] Export metadata to JSON/CSV
- [ ] Edit specific EXIF fields
- [ ] Compare metadata between images
- [ ] Dark mode theme
- [ ] RAW image format support
- [ ] Metadata visualization charts
- [ ] Print metadata report

## 💡 Use Cases

### Photography
- Analyze camera settings of professional photos
- Learn from other photographers
- Verify image authenticity

### Privacy Protection
- Remove GPS data before sharing photos
- Strip personal information from images
- Clean metadata for public posting

### Digital Forensics
- Verify image origin and authenticity
- Analyze manipulation evidence
- Track image history

### Education
- Teach photography settings
- Study exposure relationships
- Understand EXIF standards

## 🤝 Contributing

Contributions are welcome! Here's how:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines
- Keep code clean and commented
- Test on multiple browsers
- Maintain performance standards
- Update README for new features

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### MIT License Summary
✅ Commercial use  
✅ Modification  
✅ Distribution  
✅ Private use  

## 🙏 Acknowledgments

- **ExifReader** - Excellent EXIF parsing library by Mattiaz Wallander
- Icons - Inline SVG for better performance
- Color scheme inspired by modern design systems

## 📞 Support

### Getting Help
- Check the [Troubleshooting](#-troubleshooting) section
- Open an issue on GitHub
- Review closed issues for solutions

### Reporting Bugs
When reporting bugs, please include:
- Browser name and version
- Operating system
- Image format and size
- Steps to reproduce
- Error messages (if any)

## 📊 Stats

- **Lines of Code:** ~500
- **Load Time:** <1 second
- **Processing Time:** <1 second (average)
- **Dependencies:** 1 (ExifReader CDN)
- **Size:** ~15KB total (minified)

## 🌟 Star This Project

If you find this tool useful, please consider giving it a star on GitHub!

---

**Made with ❤️ for photographers, privacy advocates, and metadata enthusiasts**

**Version 2.0.0** - Last updated: February 2026

---

### Quick Links

- [Report Bug](https://github.com/YOUR-USERNAME/image-metadata-viewer/issues)
- [Request Feature](https://github.com/YOUR-USERNAME/image-metadata-viewer/issues)
- [View Demo](https://YOUR-USERNAME.github.io/image-metadata-viewer/)

---

⭐ **Star this repo if you find it useful!** ⭐
