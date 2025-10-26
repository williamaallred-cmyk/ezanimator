# Animation Maker

A web-based tool for creating simple animations with waypoints, sprite actions, and export capabilities.

## Features

- 🎨 Upload custom field images (PNG, JPG, SVG, or PDF)
- 🤖 Upload robot sprites for animations
- 📍 Click-to-add waypoints with customizable headings
- 🎬 Stop-motion style animations with multiple sprite actions per waypoint
- 🔄 Rotation control for each sprite action
- ⏸️ Pause/resume during recording with pan and zoom controls
- 💾 Export as WebM video
- 🎞️ Convert to GIF (via Cloudinary)

## How to Use

1. **Upload Files**
   - Upload a field image or PDF as the background
   - Upload an initial robot sprite

2. **Create Animation**
   - Click on the field to add waypoints
   - Select waypoints to edit heading and add sprite actions
   - Use "Add Sprite Action" to add different sprites
   - Use "Duplicate Last Action" for stop-motion effects
   - Adjust rotation for each action

3. **Record**
   - Click "Record" to start capturing
   - Press SPACE to pause/resume
   - While paused, drag to pan or scroll to zoom
   - Click "Stop Recording" when done

4. **Export**
   - Save as WebM for immediate download
   - Save as GIF for social media sharing

## Live Demo

[View Demo](#) _(Add your GitHub Pages URL here)_

## Technologies Used

- Vanilla JavaScript
- HTML5 Canvas
- MediaRecorder API
- Cloudinary API for GIF conversion
- TailwindCSS for styling
- PDF.js for PDF support

## Setup

No build process required! Just:

1. Clone the repository
2. Serve the files with any web server
3. For local testing: `npx serve` or `python -m http.server`

### Cloudinary Configuration (Optional)

For GIF conversion, configure Cloudinary in `index.html`:

```javascript
const cloudinaryConfig = {
    enabled: true,
    cloudName: 'your-cloud-name',
    uploadPreset: 'your-unsigned-preset'
};
```

## Browser Support

Works in modern browsers with:
- Canvas API
- MediaRecorder API
- Web Workers

## License

MIT License - feel free to use and modify!
