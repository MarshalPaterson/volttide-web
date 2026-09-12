# VOLTTIDE Website - Agent Guidelines

## Project Overview
This is the official website for VOLTTIDE, a psychobilly punk band. The site features:
- Band information and music promotion
- Newsletter signup form for the "Psycho Cult"
- Audio preview of their single "Taken Medication"
- Band member information
- Social media links

## File Structure
```
/ (root)
├── index.html          # Main website file
├── assets/
│   ├── TakenMedication.png  # Band artwork
│   └── TakenMedication.mp3  # Audio preview
├── .gitignore         # Git ignore rules
└── LICENSE            # MIT License
```

## Key Technologies
- HTML5
- Tailwind CSS (via CDN)
- Custom CSS for styling
- JavaScript for interactivity
- FormSubmit.co for form handling
- Font Awesome for icons

## Making Changes

### HTML Modifications
- Edit `index.html` directly for content changes
- Follow existing HTML structure and class naming conventions
- Maintain semantic HTML where possible

### CSS/Styling
- Tailwind CSS is configured in the `<script>` tag in `<head>`
- Custom CSS is in the `<style>` tag in `<head>`
- Follow existing color scheme and typography conventions:
  - Colors: voltdark, voltcard, voltgreen, voltgreenbright, voltdarkgreen, voltcream, voltdull, voltdanger
  - Fonts: horror (Creepster), punk (Permanent Marker), typewriter (Special Elite), sans (Montserrat)

### JavaScript
- Custom JavaScript is in the `<script>` tag before `</body>`
- Functions include:
  - Newsletter form handling
  - Audio preview controls
  - Mobile menu toggle
  - Presave modal
- Follow existing function naming and organization patterns

### Assets
- Images and audio files go in the `/assets/` directory
- Reference assets with relative paths like `./assets/filename.ext`

## Important Considerations

### Form Handling
- The newsletter form uses FormSubmit.co service
- The action attribute was recently updated to use a hash instead of an email address for privacy
- Do not expose email addresses directly in the code

### Responsive Design
- The site uses Tailwind's responsive classes (sm:, md:, lg:, etc.)
- Test changes at different screen sizes
- Mobile navigation uses a toggle button

### Performance
- Assets are optimized where possible
- External resources (Tailwind, Font Awesome) are loaded from CDNs
- Consider file sizes when adding new assets

## Code Conventions
- Use 2-space indentation
- Keep line lengths reasonable (< 100 characters when possible)
- Use descriptive class names that follow existing patterns
- Comments should be minimal but helpful when explaining complex logic
- Follow existing patterns for interactive elements (buttons, forms)

## Testing Changes
1. Open index.html in a browser to verify changes
2. Test form submission (note: actually submitting will send emails)
3. Test audio playback functionality
4. Verify mobile menu works correctly
5. Check responsive breakpoints

## Deployment
This is a static site that can be deployed to any static hosting service:
- Netlify
- Vercel
- GitHub Pages
- AWS S3 + CloudFront
- etc.

Simply upload the entire directory contents to the hosting service.