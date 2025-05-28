# FL Estate Pro Landing Page - Maintenance Guide

This guide will help you maintain and customize the FL Estate Pro landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions for common maintenance tasks.

## 1. Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<!-- Located at the top of the page -->
<div class="text-xl font-bold text-white">FL Estate Pro</div>
```
To change the company name, simply replace "FL Estate Pro" with your desired text.

#### Hero Section
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-6">
    Your Gateway To Florida Real Estate
</h1>
<p class="text-xl md:text-2xl text-gray-300 mb-12">
    A Remarkable Real Estate Calculator For The Sunshine State
</p>
```
Update these headings and paragraphs by replacing the text between the tags.

### Tailwind CSS Classes Explained

#### Responsive Design Classes
- `md:` - Applies styles on medium screens (768px and up)
- `lg:` - Applies styles on large screens (1024px and up)

Example:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl">
```
This heading is:
- `text-4xl` (36px) on mobile
- `text-5xl` (48px) on medium screens
- `text-6xl` (60px) on large screens

#### Common Tailwind Classes Used
- `container mx-auto`: Centers content with maximum width
- `px-6`: Horizontal padding (24px)
- `py-24`: Vertical padding (96px)
- `rounded-lg`: Rounded corners
- `hover:scale-105`: Grows element to 105% on hover
- `transition duration-300`: Smooth 300ms transitions

## 2. Fixing Broken Links

### Navigation Menu Links
Current navigation links:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

To update internal links:
1. Identify the section ID you want to link to
2. Add a `#` followed by the section ID
3. Example: `<a href="#features">Features</a>`

To add external links:
1. Replace the `#` with the full URL
2. Example: `<a href="https://example.com">External Link</a>`

### Button Links
```html
<a href="#" class="inline-block bg-gradient-to-r from-blue-500 to-purple-500">
    Get Started Now
</a>
```
Replace `#` with your desired URL or form action.

## 3. Linking Privacy and Terms Pages

### Footer Links Section
Current placeholder links:
```html
<ul class="space-y-2 text-gray-400">
    <li><a href="#" class="hover:text-white transition duration-300">Privacy Policy</a></li>
    <li><a href="#" class="hover:text-white transition duration-300">Terms of Service</a></li>
</ul>
```

To link privacy and terms pages:
1. Create your privacy.html and terms.html files
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-white transition duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition duration-300">Terms of Service</a></li>
```

## Troubleshooting Tips

### Common Issues and Solutions

1. **Broken Internal Links**
   - Ensure section IDs match exactly (case-sensitive)
   - Check for extra spaces in IDs
   - Verify the `#` is included in the href

2. **Responsive Design Issues**
   - Test on different screen sizes using browser dev tools
   - Verify media query classes (md:, lg:) are correctly placed
   - Check for conflicting responsive classes

3. **Styling Inconsistencies**
   - Copy existing classes for similar elements to maintain consistency
   - Use the same color schemes (blue-500, purple-500) for new elements
   - Maintain consistent spacing using existing padding/margin classes

### Need Help?
- Check the [Tailwind CSS documentation](https://tailwindcss.com/docs)
- Validate your HTML using [W3C Validator](https://validator.w3.org/)
- Test responsiveness using Chrome DevTools (F12)

## Best Practices

1. Always backup files before making changes
2. Test all links after updating
3. View changes on multiple devices/screen sizes
4. Maintain consistent styling across new elements
5. Keep the same color scheme and spacing patterns

Remember to update the copyright year and contact information in the footer when necessary:
```html
<p>&copy; 2024 FL Estate Pro. All rights reserved.</p>
<p class="text-gray-400">Email: rojnaweb@gmail.com</p>