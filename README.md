# Healthcare Clinic Website

A modern, responsive landing page for a doctor clinic that can be easily customized for multiple healthcare purposes.
https://muhammed-fazil-k.github.io/DoctorClinic/

## Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI/UX**: Clean, professional design with smooth animations
- **Easy Customization**: Simple HTML/CSS/JS structure for quick modifications
- **Key Sections**:
  - Hero section with call-to-action
  - Feature highlights
  - Services showcase
  - Doctor profiles
  - About section with statistics
  - Appointment booking form
  - Contact information
  - Professional footer

## Customization Guide

### 1. Change Clinic Name and Branding
Edit these sections in `index.html`:
- Line 8: `<title>` tag
- Lines 19-20: Logo and clinic name in navigation
- Line 393: Footer branding

### 2. Update Colors
Modify the CSS variables in `styles.css` (lines 5-13):
```css
:root {
    --primary-color: #2563eb;  /* Main brand color */
    --secondary-color: #10b981; /* Accent color */
    --accent-color: #f59e0b;    /* Additional accent */
}
```

### 3. Add/Remove Services
In `index.html` (lines 72-111), duplicate or remove service cards:
```html
<div class="service-card">
    <i class="fas fa-stethoscope"></i>
    <h3>Service Name</h3>
    <p>Service description</p>
</div>
```

### 4. Update Doctor Profiles
Edit the doctor cards in `index.html` (lines 120-161):
- Change names, specialties, and credentials
- Add actual photos by replacing the icon with `<img>` tags

### 5. Modify Contact Information
Update contact details in two places:
- Contact section: lines 273-299 in `index.html`
- Footer: lines 353-381 in `index.html`

### 6. Connect Form to Backend
In `script.js` (line 68), replace the console.log with your backend API:
```javascript
// Send to your backend
fetch('/api/appointments', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(data)
});
```

## File Structure

```
DoctorClinic/
├── index.html      # Main HTML structure
├── styles.css      # All styling and responsive design
├── script.js       # Interactive functionality
└── README.md       # This file
```

## Usage

1. Open `index.html` in a web browser to view the website
2. Customize the content, colors, and sections as needed
3. Deploy to any web hosting service (GitHub Pages, Netlify, Vercel, etc.)

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Technologies Used

- HTML5
- CSS3 (Grid, Flexbox, Animations)
- Vanilla JavaScript (ES6+)
- Font Awesome 6.4.0 (icons)

## Deployment

### GitHub Pages
1. Create a GitHub repository
2. Push the files to the repository
3. Enable GitHub Pages in repository settings

### Netlify
1. Drag and drop the folder to Netlify
2. Your site will be live in seconds

### Custom Server
Upload all files to your web server's public directory.

## License

Free to use for personal and commercial projects.

## Support

For questions or customization help, refer to the inline comments in each file.

---

**Created**: January 2026  
**Version**: 1.0.0
