# Obsidian CSS Snippets Collection

A collection of beautiful and functional CSS snippets to enhance your Obsidian experience with animations, colors, and improved visual effects.

## 📦 What's Included

### 🗂️ Rainbow Folder Snippets
- **Rainbow Folder Enhanced Animated** - Animated gradient folders with wave effects
- **Rainbow Folder Enhanced Solid** - Static gradient folders with clean styling

### 📅 Calendar Animations
- **Calendar Animations** - Interactive calendar day hover effects with dot pulse animations

## ✨ Features

### Rainbow Folder Enhancements
- **Colorful Gradients**: 11 different color variations that cycle through folders
- **Hover Effects**: Smooth lift and shadow animations on hover
- **Bold Typography**: Enhanced folder title styling
- **Subfolder Support**: Transparent subfolders with gray text for better hierarchy
- **Two Variants**: 
  - Animated version with moving gradients
  - Solid version for better performance

### Calendar Day Animations
- **Lift Effect**: Calendar days lift up on hover with scaling
- **Dot Pulse Animation**: Task indicator dots pulse in sequence when hovering
- **Staggered Timing**: Multiple dots animate in a wave pattern
- **Smooth Transitions**: All animations use eased timing for natural feel

## 🚀 Installation

1. **Download the CSS files** from this repository
2. **Open Obsidian** and go to Settings → Appearance
3. **Scroll down** to "CSS Snippets" section
4. **Click the folder icon** to open your snippets folder
5. **Copy the CSS files** into the snippets folder
6. **Return to Obsidian** and refresh the snippets list
7. **Toggle on** the snippets you want to use

## 📁 File Descriptions

### `Rainbow Folder enhanced animated.css`
- Creates animated gradient backgrounds for folders
- Includes continuous color shifting animation
- Best for users who enjoy dynamic visual effects
- May impact performance on slower devices

### `Rainbow Folder Enhanced solid.css`
- Static gradient backgrounds for folders
- Better performance than animated version
- Maintains all visual enhancements without animation
- Recommended for most users

### `calander animations.css`
- Interactive calendar day hover effects
- Requires a calendar plugin (like Calendar or Periodic Notes)
- Works with Svelte-based calendar implementations
- Animates task indicator dots

## 🎨 Color Palette

The folder snippets use a carefully curated color palette:
- **Pink/Rose**: `rgb(243, 139, 168)` variants
- **Peach**: `rgb(250, 179, 135)` variants  
- **Yellow**: `rgb(249, 226, 175)` variants
- **Green**: `rgb(166, 227, 161)` variants
- **Teal**: `rgb(148, 226, 213)` variants
- **Light Blue**: `rgb(137, 220, 235)` variants
- **Blue**: `rgb(116, 199, 236)` variants
- **Indigo**: `rgb(135, 176, 249)` variants
- **Purple**: `rgb(180, 190, 254)` variants
- **Lavender**: `rgb(203, 166, 247)` variants

## ⚙️ Customization

### Adjusting Colors
To change folder colors, modify the RGB values in the `:nth-child()` selectors:
```css
.nav-files-container > div > .nav-folder:nth-child(11n + 2) {
    background: linear-gradient(90deg, rgb(255, 180, 200), rgb(243, 139, 168), rgb(220, 100, 140));
}
```

### Modifying Animation Speed
For calendar animations, adjust the duration values:
```css
animation: dot-pulse 1s infinite ease-in-out; /* Change 1s to your preferred duration */
```

For folder animations, modify the keyframe duration:
```css
animation: rainbow-gradient-shift 7s ease-in-out infinite; /* Change 7s to your preferred duration */
```

### Adjusting Hover Effects
Modify the `translateY` and `scale` values to change lift intensity:
```css
transform: translateY(-5px) scale(1.02); /* Adjust -5px and 1.02 as needed */
```

## 🔧 Compatibility

### Folder Snippets
- ✅ Works with all Obsidian themes
- ✅ Compatible with custom folder structures
- ✅ Tested with AnuPpuccin theme
- ✅ Responsive design

### Calendar Animations
- ✅ Works with Calendar plugin
- ✅ Compatible with Periodic Notes
- ✅ Requires Svelte-based calendar implementation
- ⚠️ May need adjustment for custom calendar plugins

## 🐛 Troubleshooting

### Folders Not Changing Color
- Ensure the CSS snippet is enabled in Settings → Appearance
- Clear Obsidian cache and restart
- Check if another theme is overriding the styles

### Calendar Animations Not Working
- Verify you have a compatible calendar plugin installed
- Check that the calendar uses Svelte components
- Ensure the CSS class names match your calendar plugin

### Performance Issues
- Switch from animated to solid folder variant
- Reduce animation duration values
- Disable snippets on slower devices

## 📝 Credits

Created for the Obsidian community to enhance the visual experience of note-taking and organization.

## 🤝 Contributing

Feel free to:
- Report issues
- Suggest improvements
- Submit pull requests
- Share your customizations

## 📜 License

These CSS snippets are provided as-is for the Obsidian community. Feel free to modify and distribute.

---

**Enjoy your enhanced Obsidian experience!** 🎉
