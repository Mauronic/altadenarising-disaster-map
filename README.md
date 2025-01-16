
## Overview
This project provides an interactive street-view style map of Altadena, specifically documenting the areas affected by the Eaton Fire. The map allows residents and community members to view street-level imagery captured starting January 12, 2024.

![Community Photo Map Screenshot](screenshot.png)

## Purpose
This tool was specifically created to help evacuated residents:
- View their property remotely during evacuations
- Access high-resolution photos of their homes
- Easily locate properties through address search
- Share location-tagged photos with emergency services

## Features
- **Split-Screen Interface**
  - Interactive map on the right
  - Full-size photo viewer on the left
  - Responsive design for all devices

- **Intuitive Navigation**
  - Address search with autocomplete
  - Camera icons showing photo locations
  - Hover previews of photos
  - Click to view full-size images

- **Photo Viewing**
  - High-quality photo display
  - One-click access to original resolution
  - Location coordinates displayed
  - Easy close/open controls

- **Accessibility**
  - Keyboard navigation support
  - Screen reader compatible
  - High contrast mode support
  - ARIA labels throughout

## Requirements
- Web server (any static hosting will work)
- Photo data in CSV format with columns:
  - `Name`: Photo identifier/address
  - `Latitude`: GPS latitude
  - `Longitude`: GPS longitude
  - `Photo URL`: Google Drive sharing URL

## Setup
1. **Prepare Your Photos**
   ```
   - Upload photos to Google Drive
   - Set sharing permissions to "Anyone with the link can view"
   - Get the sharing URL for each photo
   ```

2. **Create Data File**
   ```
   - Create photo_data.csv
   - Add columns: Name, Latitude, Longitude, Photo URL
   - Add one row per photo
   ```

3. **Deploy**
   ```bash
   # Copy files to your web server
   cp index.html photo_data.csv /your/web/directory/
   ```

4. **Access**
   ```
   - Open in web browser
   - Photos will load automatically
   - Search or click markers to view
   ```

## Mobile Support
The interface automatically adapts to mobile devices:
- Stacks photo viewer above map
- Full-screen photo viewing
- Touch-friendly controls
- Responsive search box

## Privacy & Security
- No personal data stored
- Uses client-side processing only
- Photos served directly from Google Drive
- No tracking or analytics
- This map contains street-level imagery of public areas only. If you notice any privacy concerns, please contact us immediately at altadenarising@gmail.com. 

## Contributing
We welcome contributions! Please:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request

## License
This project is open source and available under the MIT License.

## Support
For issues or questions:
1. Open an issue in this repository
2. Provide clear steps to reproduce any problems
3. Include browser and device information

## Contact
- Email: altadenarising@gmail.com
- Website: [Altadena Rising](https://altadenarising.org)

## Acknowledgments
Built with:
- Leaflet.js for mapping
- Google Drive for photo hosting
- OpenStreetMap for base maps
- CARTO for map tiles

---

Made with ❤️ for communities in need 