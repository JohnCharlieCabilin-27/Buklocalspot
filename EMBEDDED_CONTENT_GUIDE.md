# Embedded Content Placeholder Guide

## Overview
Each of the 7 location pages now includes an **"EXPLORE MORE"** section with an embedded content placeholder where you can display external websites or online pages.

## Pages with Embedded Placeholders
1. ✅ Nasuli.html
2. ✅ Cedar.html
3. ✅ Dahilayan.html
4. ✅ Kaamulan.html
5. ✅ Kipolot.html
6. ✅ LakeApo.html
7. ✅ Communal.html
8. ✅ Sabangan.html

## How to Add External Content

### Method 1: Update the iframe `src` attribute directly
Each page has an iframe with an empty `src=""` attribute. Simply replace it with the desired website URL.

**Example:**
```html
<!-- Before (Nasuli.html) -->
<iframe id="nasuli-embed" class="embedded-iframe" src="" title="External Website for Nasuli"></iframe>

<!-- After (Nasuli.html) -->
<iframe id="nasuli-embed" class="embedded-iframe" src="https://example.com" title="External Website for Nasuli"></iframe>
```

### Supported URL Types
- ✅ **Public websites** (e.g., `https://example.com`)
- ✅ **Google Maps embeds** (e.g., `https://www.google.com/maps/embed?pb=...`)
- ✅ **YouTube embeds** (e.g., `https://www.youtube.com/embed/VIDEO_ID`)
- ✅ **Social media feeds**
- ✅ **Blog aggregators**
- ✅ **Booking/reservation systems**
- ⚠️ **Cross-origin restrictions** may apply to some websites

## Location-Specific IDs for Easy Identification

Each location has a unique iframe ID for quick reference:

| Location | File | Iframe ID |
|----------|------|-----------|
| Nasuli | Nasuli.html | `nasuli-embed` |
| Cedar | Cedar.html | `cedar-embed` |
| Dahilayan | Dahilayan.html | `dahilayan-embed` |
| Kaamulan | Kaamulan.html | `kaamulan-embed` |
| Kipolot | Kipolot.html | `kipolot-embed` |
| Lake Apo | LakeApo.html | `lakeapo-embed` |
| Communal Ranch | Communal.html | `communal-embed` |
| Sabangan | Sabangan.html | `sabangan-embed` |

## Styling & Design

### Visual Features
- **Section Title**: "EXPLORE MORE" heading with professional styling
- **Responsive iframe**: Automatically resizes based on screen size
- **Placeholder message**: Shows helpful guidance when iframe is empty
- **Dark mode support**: Automatically adapts colors in dark mode
- **Professional container**: Light gradient background with left blue border accent

### CSS Customization
If you want to modify the appearance, edit these CSS classes in `style.css`:
- `.embedded-content-section` - Main container styling
- `.iframe-placeholder` - iframe wrapper styling
- `.embedded-iframe` - iframe element styling
- `.placeholder-text` - Placeholder message styling

## Example Use Cases

### 1. Embed a Related Blog or Tourism Website
```html
<iframe id="nasuli-embed" class="embedded-iframe" src="https://www.funinthephilippines.com/nasuli-spring-resort/" title="External Website for Nasuli"></iframe>
```

### 2. Embed Google Maps Location
```html
<iframe id="cedar-embed" class="embedded-iframe" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3862.8..." title="Cedar Map"></iframe>
```

### 3. Embed YouTube Video Tour
```html
<iframe id="dahilayan-embed" class="embedded-iframe" src="https://www.youtube.com/embed/VIDEO_ID" title="Dahilayan Video Tour"></iframe>
```

### 4. Embed Booking System
```html
<iframe id="kaamulan-embed" class="embedded-iframe" src="https://booking-site.com/kaamulan-park" title="Book Kaamulan Park"></iframe>
```

## Important Notes

⚠️ **Common Issues & Solutions:**

1. **Blank iframe appearing** - Website may have CORS restrictions
   - Solution: Contact the website owner or use a different source

2. **iframe not displaying properly** - Might need height adjustment
   - Solution: The default height is 500px. Modify in style.css if needed

3. **Responsiveness issues** - Some embedded content may not be responsive
   - Solution: Check the source website's embed settings

## Quick Edit Locations

### To update all 7 pages:
- **Nasuli**: Lines 85-98
- **Cedar**: Lines 85-98
- **Dahilayan**: Lines 85-98
- **Kaamulan**: Lines 85-98
- **Kipolot**: Lines 85-98
- **LakeApo**: Lines 85-98
- **Communal**: Lines 85-98
- **Sabangan**: Lines 85-98

## Future Enhancements
Consider adding:
- Dynamic iframe URL management via JavaScript
- JavaScript function to easily update multiple iframes
- Admin panel to manage embedded content URLs
- Social media feed integration
- Real-time booking availability display

## Support
For styling or functionality questions, refer to:
- `style.css` - All embedded content styling
- Individual HTML files - iframe implementation
- HTML comments marked with `<!-- EMBEDDED CONTENT SECTION -->`
