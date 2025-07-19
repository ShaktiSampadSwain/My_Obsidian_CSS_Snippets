# Obsidian CSS Snippets Collection

A collection of beautiful and functional CSS snippets to enhance your Obsidian experience with animations, colors, and improved visual effects.
## ☕ Support Me

Did you find this Snippet useful? A little support goes a long way. Thank you!

<a href="coff.ee/Shakti_02" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
## 📦 What's Included

### 🗂️ Rainbow Folder Enhanced
- **Rainbow Folder Enhanced** - Customizable gradient folders with Style Settings plugin support
- Features both static and animated gradient options
- Fully configurable through Obsidian's Settings panel (requires Style Settings plugin)

### 📅 Calendar Animations
- **Calendar Animations** - Interactive calendar day hover effects with dot pulse animations
- Currently does not have Style Settings support (manual customization required)

## ✨ Features

### Rainbow Folder Enhanced
- **🎨 Colorful Gradients**: 11 different color variations that cycle through folders
- **⚙️ Style Settings Integration**: Full customization through Obsidian's Settings panel
- **🎭 Hover Effects**: Configurable lift and shadow animations on hover
- **💨 Performance Options**: Toggle animations on/off to optimize performance
- **🔤 Typography Control**: Adjustable font weight for folder names
- **📐 Spacing Controls**: Customizable padding and margins
- **🎯 Animation Controls**: Adjustable animation speed and effects
- **📁 Subfolder Support**: Transparent subfolders with gray text for better hierarchy

### Calendar Day Animations
- **🚀 Lift Effect**: Calendar days lift up on hover with scaling
- **💫 Dot Pulse Animation**: Task indicator dots pulse in sequence when hovering
- **🌊 Staggered Timing**: Multiple dots animate in a wave pattern
- **🎯 Smooth Transitions**: All animations use eased timing for natural feel

## 🚀 Installation

### Prerequisites
- **Style Settings Plugin** (recommended for Rainbow Folder Enhanced)
  - Install from Obsidian Community Plugins
  - Required for easy customization of Rainbow Folder Enhanced

### Installation Steps
1. **Download the CSS files** from this repository
2. **Open Obsidian** and go to Settings → Appearance
3. **Scroll down** to "CSS Snippets" section
4. **Click the folder icon** to open your snippets folder
5. **Copy the CSS files** into the snippets folder
6. **Return to Obsidian** and refresh the snippets list
7. **Toggle on** the snippets you want to use

### Style Settings Configuration
1. **Enable Style Settings plugin** (if not already installed)
2. **Navigate to Settings → Style Settings**
3. **Find "Rainbow Folder Enhanced"** in the plugin list
4. **Customize your preferences**:
   - Toggle gradient animations on/off
   - Adjust hover effects
   - Control font weight and spacing
   - Modify animation speeds
   - Set border radius and lift distances

## 📁 File Descriptions

### `Rainbow Folder Enhanced.css`
- **Style Settings Compatible**: Full integration with Style Settings plugin
- **Configurable Animations**: Toggle between static and animated gradients
- **Performance Optimized**: Choose static mode for better performance
- **Customizable Properties**: Font weight, spacing, animations, and more
- **Advanced Controls**: Border radius, lift distance, animation speed

### `calander animations.css`
- **Interactive Calendar Effects**: Hover animations for calendar days
- **Dot Pulse Animations**: Task indicator dots animate in sequence
- **Svelte Calendar Support**: Compatible with Svelte-based calendar plugins
- **Manual Customization**: Currently requires manual CSS editing for customization

## 🎨 Style Settings Options

### Rainbow Folder Enhanced Settings

#### **Animation Controls**
- **Enable Gradient Animation**: Toggle smooth gradient animations (CPU intensive)
- **Enable Hover Effects**: Toggle lift and shadow effects on hover

#### **Styling Options**
- **Folder Name Font Weight**: Control font weight (100-900)
- **Hover Lift Distance**: How far folders lift on hover (0-10px)
- **Border Radius**: Control corner roundness (0-20px)
- **Animation Speed**: Control gradient animation speed (2-15 seconds)
- **Vertical Space Between Folders**: Control spacing between folders (0-20px)
- **Vertical Padding Inside Folders**: Control internal padding (1-20px)

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

## ⚙️ Manual Customization

### Calendar Animations (Manual Only)
Since calendar animations don't have Style Settings support yet, you can manually customize:

#### Adjusting Animation Speed
```css
animation: dot-pulse 1s infinite ease-in-out; /* Change 1s to your preferred duration */
```

#### Modifying Hover Effects
```css
transform: translateY(-5px) scale(1.02); /* Adjust -5px and 1.02 as needed */
```

#### Changing Dot Animation Delays
```css
animation-delay: 0.10s; /* Adjust delay for staggered effect */
```

### Rainbow Folder Enhanced (Advanced Manual Customization)
While Style Settings provides most customization options, you can still manually edit:

#### Custom Colors
```css
.nav-files-container > div > .nav-folder:nth-child(11n + 2) {
    background: linear-gradient(90deg, rgb(255, 180, 200), rgb(243, 139, 168), rgb(220, 100, 140));
}
```

## 🔧 Compatibility

### Rainbow Folder Enhanced
- ✅ **Style Settings Plugin**: Full integration and support
- ✅ **All Obsidian Themes**: Works with any theme
- ✅ **Custom Folder Structures**: Compatible with nested folders
- ✅ **Performance Optimized**: Configurable animations for different device capabilities
- ✅ **Responsive Design**: Adapts to different screen sizes

### Calendar Animations
- ✅ **Calendar Plugin**: Works with official Calendar plugin
- ✅ **Periodic Notes**: Compatible with Periodic Notes plugin
- ✅ **Svelte-based Calendars**: Requires Svelte calendar implementation
- ⚠️ **Custom Calendar Plugins**: May need adjustment for non-standard plugins

## 🐛 Troubleshooting

### Rainbow Folder Enhanced
- **Colors Not Appearing**: Check if snippet is enabled and Style Settings plugin is installed
- **Settings Not Showing**: Ensure Style Settings plugin is installed and active
- **Performance Issues**: Disable gradient animations in Style Settings
- **Folders Not Styling**: Clear Obsidian cache and restart

### Calendar Animations
- **Animations Not Working**: Verify compatible calendar plugin is installed
- **Dots Not Pulsing**: Check that calendar uses Svelte components
- **Performance Issues**: Reduce animation duration in CSS manually

### General Issues
- **Snippet Not Loading**: Refresh snippets list in Appearance settings
- **Conflicts with Theme**: Try disabling other CSS snippets temporarily
- **Performance Problems**: Use Style Settings to reduce animation effects

## 📋 Requirements

### Essential
- **Obsidian**: Latest version recommended
- **CSS Snippets Support**: Built into Obsidian

### Recommended
- **Style Settings Plugin**: For easy Rainbow Folder Enhanced customization
- **Calendar Plugin**: For calendar animations to work
- **Periodic Notes Plugin**: Enhances calendar functionality

## 🎯 Performance Tips

### For Slower Devices
1. **Disable Gradient Animations**: Use Style Settings to turn off animations
2. **Reduce Hover Effects**: Lower lift distance and disable shadows
3. **Minimize Animation Speed**: Set longer animation durations
4. **Use Static Mode**: Keep animations disabled for better performance

### For Better Performance
1. **Enable Hardware Acceleration**: In Obsidian settings
2. **Close Unnecessary Plugins**: Reduce overall resource usage
3. **Restart Obsidian**: After making significant changes
4. **Update Regularly**: Keep Obsidian and plugins updated

## 🔄 Future Updates

### Planned Features
- **Style Settings support for Calendar Animations**
- **Additional color schemes for folders**
- **More calendar animation options**
- **Theme-specific optimizations**

### Contribution Ideas
- Custom color palette suggestions
- Performance optimization improvements
- Additional animation effects
- Theme compatibility testing

## 📝 Credits

Created for the Obsidian community to enhance the visual experience of note-taking and organization.

Special thanks to:
- **Style Settings Plugin developers** for making customization accessible
- **Obsidian community** for feedback and suggestions
- **Calendar plugin developers** for creating compatible interfaces

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Ways to Contribute
- **Report Issues**: Found a bug? Let us know!
- **Suggest Features**: Have ideas for improvements?
- **Submit Pull Requests**: Code improvements and new features
- **Share Customizations**: Show off your modifications
- **Test Compatibility**: Help test with different themes and plugins

### Development Guidelines
- **Comment Your Code**: Make it easy for others to understand
- **Test Thoroughly**: Ensure compatibility across different setups
- **Follow CSS Best Practices**: Maintain clean, efficient code
- **Document Changes**: Update README with new features

## 📜 License

These CSS snippets are provided as-is for the Obsidian community. Feel free to modify, distribute, and build upon them.

## 🆘 Support

Need help? Here are your options:

1. **Check Troubleshooting Section**: Common issues and solutions
2. **Style Settings Documentation**: For plugin-specific help
3. **Obsidian Community**: Discord and forum support
4. **GitHub Issues**: Report bugs and request features

---

**Enjoy your enhanced Obsidian experience!** 🎉

> **Pro Tip**: Start with Style Settings for Rainbow Folder Enhanced to easily customize your setup, then explore manual customization for advanced tweaks!
