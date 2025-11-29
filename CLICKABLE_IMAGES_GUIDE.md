# External Content Links - Image-Based Implementation

## ✅ Changes Completed

All 8 location pages have been updated with **clickable image cards** instead of iframes:

1. ✅ Nasuli.html
2. ✅ Cedar.html
3. ✅ Dahilayan.html
4. ✅ Kaamulan.html
5. ✅ Kipolot.html
6. ✅ LakeApo.html
7. ✅ Communal.html
8. ✅ Sabangan.html

## New Features

### Visual Design
- **3-column responsive grid** - Images adapt to screen size (minimum 200px width)
- **Smaller images** - Each card is 200px tall with professional aspect ratio
- **Hover effects** - Images lift up and brighten on hover
- **Interactive overlays** - Emojis and text labels appear on hover
- **Smooth animations** - 0.3s transitions for all interactions
- **Professional styling** - Rounded corners, shadows, and gradients

### Functionality
- **Clickable cards** - Click anywhere on the image to open the link
- **External links** - All links open in new tabs (`target="_blank"`)
- **Three links per location**:
  1. 🔗 Travel guide/blog website
  2. 📍 Google Maps location
  3. ➕ Placeholder for user to add custom link

### User Experience
- **Help text** - "💡 Click on any image to visit the external website or map location"
- **Easy identification** - Each card shows what it links to via overlay icons
- **Dark mode support** - Automatically adapts styling in dark mode
- **Responsive** - Works on mobile, tablet, and desktop

## How to Add More Links

To add a custom link to any location, replace the placeholder `<a>` tag:

```html
<!-- Find this section in the HTML: -->
<a href="#" class="external-link-card" title="Add your external link here">
  <img src="IMAGE_URL" alt="Add External Link">
  <div class="link-overlay">
    <span class="link-icon">➕</span>
    <p>Add Link</p>
  </div>
</a>

<!-- Change to: -->
<a href="https://your-website.com" target="_blank" class="external-link-card">
  <img src="https://image-url.jpg" alt="Your Description">
  <div class="link-overlay">
    <span class="link-icon">🔗</span>
    <p>Your Link Name</p>
  </div>
</a>
```

## CSS Classes Reference

| Class | Purpose |
|-------|---------|
| `.embedded-content-section` | Main container with gradient background |
| `.external-links-grid` | Responsive grid layout |
| `.external-link-card` | Individual card with hover effects |
| `.link-overlay` | Dark overlay that appears on hover |
| `.external-links-help` | Help text below the grid |

## Image Sizing

- **Card height**: 200px (responsive width)
- **Grid columns**: Auto-fit with minimum 200px width
- **Images**: Scale to fill container (object-fit: cover)
- **Aspect ratio**: Maintains natural image proportions

## Hover Effects

1. **Image**: Lifts up 8px and scales up 2% (`translateY(-8px) scale(1.02)`)
2. **Shadow**: Darkens from 0.1 to 0.2 opacity
3. **Brightness**: Reduces to 70% brightness
4. **Overlay**: Fades in with link icon and label

## Browser Compatibility

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers

## Styling Customization

To modify appearance, edit these in `style.css`:

```css
.external-link-card {
  height: 200px;  /* Card height */
  border-radius: 10px;  /* Corner roundness */
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);  /* Shadow depth */
}

.external-links-grid {
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));  /* Column width */
  gap: 20px;  /* Space between cards */
}
```

## Current External Links by Location

| Location | Link 1 | Link 2 |
|----------|--------|--------|
| Nasuli | meanttogo.com | Google Maps |
| Cedar | wanderingfeetph.com | Google Maps |
| Dahilayan | realbreezedavaotours.com | Google Maps |
| Kaamulan | waze.com | Google Maps |
| Kipolot | graciestrips.wordpress.com | Google Maps |
| Lake Apo | meanttogo.com | Google Maps |
| Communal | escapemanila.com | Google Maps |
| Sabangan | Google Maps | Google Maps |

All locations have a third placeholder card ready for custom links!
