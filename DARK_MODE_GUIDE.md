# Dark Mode & Loading Screen Features

## 🌓 Dark Mode Toggle

### Features Added:
- **Toggle Button**: Located in the navigation bar (moon/sun icon)
- **Local Storage**: Remembers user preference across sessions
- **Smooth Transitions**: All elements transition smoothly between modes
- **Automatic Icon Change**: Moon icon in light mode, sun icon in dark mode

### How It Works:
1. Click the moon/sun icon in the navigation bar
2. The entire site switches between light and dark modes
3. Your preference is saved in browser local storage
4. The site will remember your choice on your next visit

### Dark Mode Colors:
- **Background**: Dark grays (#111827, #1f2937)
- **Text**: Light colors (#f9fafb, #d1d5db)
- **Borders**: Subtle dark borders (#374151)
- **Accents**: Same vibrant blues maintained

### Customization:
To adjust dark mode colors, edit in `css/style.css`:
```css
body.dark-mode {
    --text-primary: #f9fafb;
    --text-secondary: #d1d5db;
    --bg-light: #1f2937;
    --bg-white: #111827;
    --border-color: #374151;
}
```

## ⏳ Loading Screen Animation

### Features Added:
- **Branded Logo**: Displays your name with gradient effect
- **Spinning Loader**: Animated spinner during load
- **Loading Text**: "Loading Portfolio..." with pulse animation
- **Smooth Fade Out**: Elegant transition to main content
- **Minimum Display Time**: Shows for at least 1.5 seconds

### Loading Screen Elements:
1. **Logo Animation**: Fades in from bottom
2. **Spinner**: Continuous rotation with brand colors
3. **Text**: Pulsing opacity effect
4. **Background**: Matches current theme (light/dark)

### Customization:

**Change Loading Duration** (`js/script.js`):
```javascript
setTimeout(() => {
    loadingScreen.classList.add('hidden');
}, 1500); // Change this value (milliseconds)
```

**Modify Loading Text** (`index.html`):
```html
<p class="loader-text">Loading Portfolio...</p>
```

**Adjust Spinner Speed** (`css/style.css`):
```css
@keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
}
/* Change animation duration in .spinner class */
animation: spin 1s linear infinite; /* Adjust 1s for speed */
```

## 🎨 Visual Enhancements

### Smooth Transitions:
All elements now have smooth transitions when switching themes:
- Cards and containers
- Text colors
- Background colors
- Borders and shadows
- Icons and buttons

### Responsive Design:
Both features work seamlessly on all devices:
- Desktop: Full-size toggle button
- Tablet: Optimized button size
- Mobile: Compact toggle next to hamburger menu

## 🔧 Technical Details

### Files Modified:
1. **index.html**
   - Added loading screen HTML structure
   - Added dark mode toggle button in navigation

2. **css/style.css**
   - Added CSS variables for dark mode
   - Added loading screen styles and animations
   - Added dark mode specific styles for all components
   - Added smooth transition properties

3. **js/script.js**
   - Added loading screen functionality
   - Added dark mode toggle with local storage
   - Added preference persistence

### Browser Compatibility:
- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Opera (latest)

### Performance:
- Lightweight: Minimal JavaScript (~50 lines added)
- CSS-based animations for smooth performance
- Local storage for instant preference loading
- No external dependencies

## 🐛 Troubleshooting

**Dark mode not saving:**
- Check if browser allows local storage
- Clear cache and try again
- Check browser console for errors

**Loading screen doesn't disappear:**
- Check JavaScript console for errors
- Ensure `loadingScreen` ID exists in HTML
- Verify JavaScript file is loaded correctly

**Toggle button not visible:**
- Check if screen width is below 768px (mobile view)
- Look for button in hamburger menu area
- Verify CSS file is loaded

## 📱 Mobile Experience

On mobile devices:
- Dark mode toggle appears next to hamburger menu
- Slightly smaller button size for better fit
- Touch-friendly 35x35px tap target
- Same smooth transitions

## 🎯 Best Practices

1. **Testing**: Test on different devices and browsers
2. **Colors**: Ensure sufficient contrast in both modes
3. **Images**: Consider using different images for dark mode if needed
4. **Performance**: Loading screen shows minimum 1.5s to avoid flicker

## 🚀 Future Enhancements

Possible additions:
- [ ] System preference detection (auto dark mode)
- [ ] Custom loading messages
- [ ] Loading progress bar
- [ ] Smooth theme transition animation
- [ ] Custom color schemes (blue, purple, green themes)

## 📞 Support

If you encounter any issues:
1. Check browser console for errors
2. Verify all files are properly linked
3. Clear browser cache
4. Test in incognito/private mode

---

Made with ❤️ by Leo Melo
