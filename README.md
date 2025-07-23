# Einurm Website

Modern static website for Einurm - Estonian furniture assembly company. Built with HTML, Tailwind CSS, and vanilla JavaScript.

## Structure

- `index.html` - Home page (Esileht + Meist)
- `hinnakiri.html` - Pricing page
- `koostoopartnerid.html` - Partners page  
- `kontakt.html` - Contact page with form

## Features

- **Responsive Design**: Works on all devices (mobile, tablet, desktop)
- **Modern UI**: Clean, professional design using Tailwind CSS
- **Fast Loading**: Uses Tailwind CSS via CDN for quick loading
- **GitHub Pages Ready**: Static HTML files that work perfectly with GitHub Pages
- **Interactive Elements**: 
  - Mobile navigation menu
  - Contact form with validation
  - FAQ accordion
  - Hover effects and transitions

## GitHub Pages Deployment

1. Create a new repository on GitHub
2. Upload all the HTML files to the repository
3. Go to repository Settings > Pages
4. Select "Deploy from a branch" and choose "main" branch
5. Your site will be available at `https://yourusername.github.io/repositoryname`

## Customization Guide

### Adding Partner Logos

1. Add logo images to a `images/partners/` folder
2. Replace the placeholder divs in `koostoopartnerid.html` with:
```html
<div class="bg-white rounded-lg shadow-md p-8 flex items-center justify-center min-h-32 hover:shadow-lg transition-shadow">
    <a href="https://partner-website.com" target="_blank">
        <img src="images/partners/partner-logo.png" alt="Partner Name" class="max-h-16 max-w-full object-contain">
    </a>
</div>
```

### Updating Contact Information

Replace placeholder contact details in `kontakt.html`:
- Phone numbers: Replace `+372 XXXX XXXX` with actual numbers
- Email: Replace `info@einurm.ee` with actual email
- Update the footer contact info across all pages

### Modifying Colors

The website uses a custom color scheme defined in the Tailwind config:
- `einurm-blue`: #1e40af (main brand color)
- `einurm-gray`: #6b7280 (secondary text color)

To change colors, modify the `tailwind.config` section in each HTML file.

### Adding Content

- **Images**: Create an `images/` folder and add photos of completed work
- **Testimonials**: Add customer reviews to the home page
- **Gallery**: Create a new page showcasing completed projects

## Browser Support

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Internet Explorer 11+ (with some limitations)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance

- **Lightweight**: No heavy frameworks or libraries
- **Fast CDN**: Tailwind CSS loaded from fast CDN
- **Optimized**: Minimal JavaScript for better performance
- **SEO Friendly**: Semantic HTML structure

## Form Handling

The contact form currently shows a JavaScript alert when submitted. For production, you'll need to:

1. **Use a form service** like Netlify Forms, Formspree, or EmailJS
2. **Add server-side processing** if you have backend capabilities
3. **Integrate with email services** for automatic notifications

### Example with Formspree:

```html
<form action="https://formspree.io/f/your-form-id" method="POST">
    <!-- form fields -->
</form>
```

## Maintenance

- **Regular Updates**: Update phone numbers, prices, and content as needed
- **Content Review**: Keep the "about" section and services list current
- **Link Checking**: Ensure all internal and external links work
- **Image Optimization**: Compress images for faster loading

## Technical Notes

- Uses semantic HTML5 for better accessibility
- Mobile-first responsive design approach
- CSS Grid and Flexbox for layouts
- Smooth transitions and hover effects
- Print-friendly styles (basic support)

## Future Enhancements

Consider adding:
- **Image gallery** with lightbox functionality
- **Before/after project photos**
- **Customer testimonials** section
- **Blog/news** section for updates
- **Online booking** system integration
- **Multi-language** support (Estonian/English)

## Support

For technical questions about the website code, refer to:
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [MDN Web Docs](https://developer.mozilla.org/en-US/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
# einurm-static
