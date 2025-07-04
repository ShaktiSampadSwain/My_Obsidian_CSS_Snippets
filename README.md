# Obsidian Enhanced Folder & File Styling Snippet

This CSS snippet for Obsidian enhances the visual appeal and user experience of your file explorer by adding vibrant, animated gradient backgrounds to folders, subtle hover effects, clear bold text for folder names, and distinct highlighting for files.

![darkmode](https://github.com/ShaktiSampadSwain/RainbowFolderObsidian/blob/main/rainbowfolderDark.png)
## ✨ Features

- **Animated Gradient Folder Backgrounds:** Each top-level folder features a unique, slowly animating gradient background, creating a dynamic and visually engaging file explorer.
    
- **Customizable Color Palettes:** Easily define the light, base, and dark shades for each folder's gradient using CSS custom properties (`--folder-color-light`, `--folder-color`, `--folder-color-dark`).
    
- **Consistent Subfolder Styling:** Subfolders inherit the same animated gradient and color scheme based on their position within their parent, maintaining visual consistency across nested levels.
    
- **Bold Folder Names:** Folder titles are explicitly bolded for improved readability and distinction.
    
- **Subtle Gray Subfolder Titles:** Subfolder names are shaded gray, providing a clear visual hierarchy.
    
- **Clean Hover Effects:** Folders subtly lift and gain a shadow on hover, offering clear interactive feedback without distracting background changes or text blurring.
    
- **File Name Highlighting:** Files display a gentle background highlight when hovered, making them easy to identify.
    
- **No Text Shadow:** Text shadows have been removed for a cleaner, sharper text appearance.
    

## 🚀 Installation

1. **Open Obsidian:** Launch your Obsidian application.
    
2. **Go to Settings:** Click the gear icon (Settings) in the bottom-left corner.
    
3. **Navigate to Appearance:** In the settings sidebar, click on "Appearance."
    
4. **Enable CSS Snippets:** Scroll down to the "CSS snippets" section. If it's not already enabled, toggle it on.
    
5. **Open Snippets Folder:** Click the folder icon next to "CSS snippets" to open the `snippets` folder in your vault.
    
6. **Create a New File:** Inside this `snippets` folder, create a new `.css` file (e.g., `enhanced-folders.css`).
    
7. **Paste the Code:** Copy the entire CSS code provided below and paste it into this new `.css` file. Save the file.
    
8. **Enable the Snippet:** Go back to Obsidian's Appearance settings. Under "CSS snippets," you should now see your new snippet file. Toggle it on.
    

Your file explorer should now display the enhanced styling!

## 📋 The Code

```css
/* Base folder style with animated gradient background */
.nav-files-container > div > .nav-folder {
    background: linear-gradient(90deg, var(--folder-color-light), var(--folder-color), var(--folder-color-dark));
    background-size: 300% 300%;
    animation: rainbow-gradient-shift 7s ease-in-out infinite;
    --nav-item-color: black;
    --nav-item-color-hover: black;
    --nav-collapse-icon-color: black;
    border-radius: 10px;
    padding: 5px 10px;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
    margin-bottom: 6px;
    transition: all 0.2s ease-in-out;
    filter: brightness(0.95);
}

/* Folder title bold */
.nav-files-container > div > .nav-folder-title {
    font-weight: bold !important ;
    background-color: transparent !important;
}

/* Hover effect */
.nav-files-container > div > .nav-folder:hover {
    filter: brightness(1);
    transform: translateY(-3px);
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

/* Folder-specific color variables */
.nav-files-container > div > .nav-folder:nth-child(11n + 2) {
    --folder-color: rgb(243, 139, 168);
    --folder-color-light: rgb(255, 180, 200);
    --folder-color-dark: rgb(220, 100, 140);
}

.nav-files-container > div > .nav-folder:nth-child(11n + 3) {
    --folder-color: rgb(235, 160, 172);
    --folder-color-light: rgb(255, 190, 200);
    --folder-color-dark: rgb(210, 120, 140);
}

.nav-files-container > div > .nav-folder:nth-child(11n + 4) {
    --folder-color: rgb(250, 179, 135);
    --folder-color-light: rgb(255, 210, 170);
    --folder-color-dark: rgb(230, 140, 100);
}

.nav-files-container > div > .nav-folder:nth-child(11n + 5) {
    --folder-color: rgb(249, 226, 175);
    --folder-color-light: rgb(255, 245, 210);
    --folder-color-dark: rgb(220, 190, 130);
}

.nav-files-container > div > .nav-folder:nth-child(11n + 6) {
    --folder-color: rgb(166, 227, 161);
    --folder-color-light: rgb(200, 250, 190);
    --folder-color-dark: rgb(130, 190, 130);
}

.nav-files-container > div > .nav-folder:nth-child(11n + 7) {
    --folder-color: rgb(148, 226, 213);
    --folder-color-light: rgb(180, 250, 240);
    --folder-color-dark: rgb(110, 190, 180);
}

.nav-files-container > div > .nav-folder:nth-child(11n + 8) {
    --folder-color: rgb(137, 220, 235);
    --folder-color-light: rgb(170, 240, 250);
    --folder-color-dark: rgb(100, 180, 200);
}

.nav-files-container > div > .nav-folder:nth-child(11n + 9) {
    --folder-color: rgb(116, 199, 236);
    --folder-color-light: rgb(150, 220, 250);
    --folder-color-dark: rgb(80, 160, 200);
}

.nav-files-container > div > .nav-folder:nth-child(11n + 10) {
    --folder-color: rgb(135, 176, 249);
    --folder-color-light: rgb(170, 200, 255);
    --folder-color-dark: rgb(100, 140, 210);
}

.nav-files-container > div > .nav-folder:nth-child(11n + 11) {
    --folder-color: rgb(180, 190, 254);
    --folder-color-light: rgb(210, 220, 255);
    --folder-color-dark: rgb(140, 150, 220);
}

.nav-files-container > div > .nav-folder:nth-child(11n + 12) {
    --folder-color: rgb(203, 166, 247);
    --folder-color-light: rgb(230, 200, 255);
    --folder-color-dark: rgb(160, 120, 210);
}

/* Gradient animation keyframes */
@keyframes rainbow-gradient-shift {
    0% {
        background-position: 0% 50%;
    }
    50% {
        background-position: 100% 50%;
    }
    100% {
        background-position: 0% 50%;
    }
}

/* Bold folder names (applies to text within any .nav-folder) */
.nav-files-container .nav-folder-title .nav-file-title-content,
.nav-files-container .nav-folder-title .nav-folder-title-content {
    font-weight: 500 !important;
    position: relative;
    z-index: 2;
    color: var(--nav-item-color) !important;
    text-shadow: none !important; /* No text shadow */
    background-color: transparent !important;
    transition: background-color 0.1s ease;
}

/* Subfolder Title Gray Shading */
.nav-files-container .nav-folder-children .nav-folder-title .nav-folder-title-content {
    color: rgba(0, 0, 0, 0.8) !important;
    text-shadow: none !important;
}

/* Ensure collapse icon is above gradient (applies to icons within any .nav-folder) */
.nav-files-container .nav-folder-title .nav-folder-collapse-icon {
    position: relative;
    z-index: 2;
    color: var(--nav-collapse-icon-color) !important;
}

/* Hover effect for ANY folder container (main or subfolder) */
.nav-files-container .nav-folder:hover {
    transform: translateY(-3px); /* Lifts the folder */
    box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1); /* Pop-out shadow on hover */
}

/* Highlight for File Names on Hover */
.nav-files-container .nav-file:hover .nav-file-title-content {
    background-color: rgba(0, 0, 0, 0.1); /* Subtle black highlight */
    border-radius: 4px; /* Rounded corners for the highlight */
    padding: 0 4px; /* Add some padding around the text */
    margin: 0 -4px; /* Compensate for padding to keep alignment */
}

/* Ensure folder names do NOT get highlighted */
.nav-files-container .nav-folder-title:hover .nav-folder-title-content {
    background-color: transparent !important;
}

/* AnuPpuccin theme specific overrides (if necessary, keep these at the end) */
/* This ensures font consistency if the theme tries to override it */
.theme-anupucin .nav-files-container .nav-folder-title .nav-file-title-content,
.theme-anupucin .nav-files-container .nav-folder-title .nav-folder-title-content {
    font-family: 'Inter', 'Segoe UI', system-ui, -apple-system, BlinkMacSystemFont, sans-serif !important;
}
```

## 💡 Code Explanation

This snippet primarily targets elements within Obsidian's file explorer (`.nav-files-container`) to apply custom styling.

### 1. Base Folder Styling (`.nav-files-container > div > .nav-folder`)

This section defines the core appearance and behavior for all top-level folders.

- `background: linear-gradient(...)`: Creates a gradient background for each folder. It uses three CSS custom properties (`--folder-color-light`, `--folder-color`, `--folder-color-dark`) to define the specific shades for each folder, which are set later by `nth-child` rules.
    
- `background-size: 300% 300%;`: Makes the gradient three times larger than the folder, allowing for a smooth, continuous animation as its position shifts.
    
- `animation: rainbow-gradient-shift 7s ease-in-out infinite;`: Applies the animation defined by `@keyframes rainbow-gradient-shift`.
    
    - `7s`: The duration of one complete animation cycle.
        
    - `ease-in-out`: Provides a smooth start and end to the animation.
        
    - `infinite`: Makes the animation loop continuously.
        
- `--nav-item-color`, `--nav-item-color-hover`, `--nav-collapse-icon-color`: Custom properties to define the text and icon colors, ensuring high contrast against the folder backgrounds.
    
- `border-radius: 10px;`: Rounds the corners of the folders.
    
- `padding: 5px 10px;`: Adds space around the folder content.
    
- `overflow: hidden;`: Ensures any content or effects stay within the rounded borders.
    
- `text-overflow: ellipsis; white-space: nowrap;`: Handles long folder names by truncating them with an ellipsis (...).
    
- `margin-bottom: 6px;`: Provides vertical spacing between folders.
    
- `transition: all 0.2s ease-in-out;`: Smooths transitions for properties like `transform` and `box-shadow` on hover.
    
- `filter: brightness(0.95);`: Slightly darkens the default appearance of the folder background.
    

### 2. Folder Title Boldness (`.nav-files-container > div > .nav-folder-title`)

This rule ensures the main folder titles are bold.

- `font-weight: bold !important;`: Makes the folder title text bold, using `!important` to override potential theme conflicts.
    
- `background-color: transparent !important;`: Ensures no background color is applied directly to the title itself, preventing unwanted highlights.
    

### 3. Hover Effect (`.nav-files-container > div > .nav-folder:hover`)

This section defines the visual feedback when you hover over any folder.

- `filter: brightness(1);`: On hover, the folder's brightness returns to normal (from the `0.95` default), making it slightly brighter.
    
- `transform: translateY(-3px);`: Lifts the folder slightly upwards, creating a "pop-out" effect.
    
- `box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);`: Adds a subtle shadow beneath the lifted folder, enhancing the sense of depth.
    

### 4. Folder-Specific Color Variables (`.nav-files-container > div > .nav-folder:nth-child(...)`)

These rules use the `nth-child` pseudo-class to assign a unique set of `light`, `base`, and `dark` colors (via custom properties) to every 11th folder in the list. This creates the rainbow-like, distinct color scheme for your top-level folders.

- `--folder-color`: The main color of the folder.
    
- `--folder-color-light`: A lighter shade of the main color.
    
- `--folder-color-dark`: A darker shade of the main color.
    
- `nth-child(11n + X)`: This CSS selector pattern cycles through 11 different styles. `11n + 2` applies to the 2nd, 13th, 24th, etc., folder. This ensures a repeating pattern of distinct colors.
    

### 5. Gradient Animation Keyframes (`@keyframes rainbow-gradient-shift`)

This defines how the gradient background animates.

- `0% { background-position: 0% 50%; }`: Starts the gradient at the left edge.
    
- `50% { background-position: 100% 50%; }`: Moves the gradient to the right edge at the halfway point.
    
- `100% { background-position: 0% 50%; }`: Moves the gradient back to the left edge, completing the cycle. The `infinite alternate` in the `animation` property (defined in the base folder style) makes it smoothly reverse direction, creating a continuous ebb and flow.
    

### 6. Subfolder Title Gray Shading (`.nav-files-container .nav-folder-children .nav-folder-title .nav-folder-title-content`)

This section specifically targets subfolder titles to make them appear gray, creating a visual hierarchy.

- `color: rgba(0, 0, 0, 0.8) !important;`: Sets the text color to a semi-transparent black, resulting in a gray appearance.
    
- `text-shadow: none !important;`: Ensures no text shadow is applied to subfolder titles for a cleaner look.
    

### 7. File Name Highlighting (`.nav-files-container .nav-file:hover .nav-file-title-content`)

This rule provides visual feedback when hovering over individual files.

- `background-color: rgba(0, 0, 0, 0.1);`: Applies a subtle, semi-transparent black background highlight to the file name.
    
- `border-radius: 4px;`: Rounds the corners of the highlight.
    
- `padding: 0 4px; margin: 0 -4px;`: Adjusts the spacing to make the highlight extend slightly beyond the text without affecting layout.
    

### 8. Compatibility Overrides (e.g., `.theme-anupucin ...`)

These sections are included to address potential conflicts with specific Obsidian themes, such as "AnuPpuccin." They ensure that the desired font-weight and font-family are applied consistently, overriding theme defaults if necessary.

## ⚙️ Customization

- **Folder Colors:** Modify the `rgb()` values for `--folder-color`, `--folder-color-light`, and `--folder-color-dark` in each `nth-child` block to change the color palette of your folders.
    
- **Animation Speed:** Adjust the `7s` value in `animation: rainbow-gradient-shift 7s ease-in-out infinite;` to make the gradient animation faster or slower.
    
- **Hover Effect Intensity:**
    
    - Change `transform: translateY(-3px);` to a different pixel value for more or less lift.
        
    - Adjust `box-shadow` values (`0 6px 15px rgba(0, 0, 0, 0.1)`) for a softer or stronger shadow.
        
    - Modify `filter: brightness(1);` on hover to make the folder brighter or darker.
        
- **Subfolder Gray Shade:** Change the `rgba(0, 0, 0, 0.8)` value in the `.nav-files-container .nav-folder-children .nav-folder-title .nav-folder-title-content` rule to make subfolder text lighter or darker.
    
- **File Highlight:** Adjust `rgba(0, 0, 0, 0.1)` in `.nav-files-container .nav-file:hover .nav-file-title-content` for a more or less opaque file highlight.
