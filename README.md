Obsidian CSS Snippets: Interactive UI Enhancements
This repository contains a collection of CSS snippets designed to enhance the visual appeal and interactivity of your Obsidian vault. From dynamic folder styling to animated calendar dates, these snippets aim to create a more engaging and personalized note-taking experience.

🚀 Features
This repository includes the following distinct CSS snippets:

📁 Enhanced Folder & File Styling
This snippet transforms your Obsidian file explorer with vibrant backgrounds and clear visual cues. It offers two main variants:

Animated Gradient Folder Backgrounds: Top-level folders feature unique, slowly animating gradient backgrounds for a dynamic file explorer.

Solid Gradient Folder Backgrounds: Top-level folders display fixed, non-animating gradient backgrounds, offering a more subtle but still colorful appearance.

Both variants share these common features:

Customizable Color Palettes: Easily define light, base, and dark shades for each folder's gradient using CSS custom properties.

Consistent Subfolder Styling: Subfolders inherit the same color scheme (or are transparent in the solid variant) based on their parent, maintaining visual consistency.

Bold Folder Names: Folder titles are explicitly bolded for improved readability.

Subtle Gray Subfolder Titles: Subfolder names are shaded gray, providing a clear visual hierarchy.

Clean Hover Effects: Folders subtly lift and gain a shadow on hover, offering clear interactive feedback.

File Name Highlighting: Files display a gentle background highlight when hovered, making them easy to identify.

No Text Shadow: Text shadows have been removed for a cleaner, sharper text appearance.

📅 Interactive Calendar Animations
This snippet adds subtle "lift" and "pulse" animations to dates and their associated note indicators (dots) within the Obsidian Calendar plugin (Liam Cain's plugin).

Date Lift Effect: When you hover over any date in the calendar, the entire date cell gently lifts up and casts a subtle shadow, creating a three-dimensional pop-out effect.

Dynamic Dot Pulse Animation: For dates with multiple note indicators (dots), hovering over the date triggers a "loading screen" or "wave" animation where the filled dots expand and contract in quick succession. The hollow dot (if present) remains static.

💡 Installation
To use these snippets in your Obsidian vault:

Open Obsidian.

Go to Settings (the gear icon in the bottom-left corner).

Navigate to Appearance in the sidebar.

Scroll down to the CSS snippets section. If it's not already enabled, toggle it on.

Click the folder icon next to "CSS snippets" to open the snippets folder in your vault.

For each snippet you want to use:

Create a new .css file inside this snippets folder (e.g., enhanced-folders-animated.css for the animated folder styling, enhanced-folders-solid.css for the solid folder styling, calendar-animations.css for the calendar animations).

Copy the entire CSS code for that specific snippet (provided in the sections below) and paste it into its respective new .css file. Save the file.

Go back to Obsidian's Appearance settings. Under "CSS snippets," you should now see your new snippet files listed. Toggle each one on that you wish to activate.

Restart Obsidian for the changes to take full effect, especially for animations.

🎨 Visual Examples (Folder & File Styling)
These images demonstrate the "Enhanced Folder & File Styling" snippet in action (specifically the animated gradient variant):

(Note: Calendar animations are dynamic and best experienced live in Obsidian.)

📋 CSS Snippets
📁 Enhanced Folder & File Styling Snippet (Animated Gradient)
This snippet provides folders with a continuously animating gradient background.

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

📁 Enhanced Folder & File Styling Snippet (Solid Gradient)
This snippet provides folders with a static, non-animating gradient background.

/* Finalized Obsidian Folder & File Styling Snippet v11.0 */
/* Top-level folders have fixed gradient backgrounds.
   Subfolders are transparent (no background).
   Maintains bold text, gray subfolder titles, and refined hover/highlight behaviors. */

/* Base folder styling (applies to all .nav-folder elements) */
.nav-files-container .nav-folder {
    --nav-item-color: black;
    --nav-item-color-hover: black;
    --nav-collapse-icon-color: black;

    position: relative;
    border-radius: 10px;
    padding: 5px 10px;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
    margin-bottom: 6px;
    transition: all 0.2s ease-in-out; /* Keep transition for hover effects */
    filter: brightness(0.95); /* Keep initial brightness */

    border: none;
    box-shadow: none;
}

/* Folder title bold */
.nav-files-container .nav-folder-title { /* General selector for all folder titles */
    font-weight: bold !important;
    background-color: transparent !important;
}

/* Hover effect for ANY folder container (main or subfolder) */
.nav-files-container .nav-folder:hover {
    filter: brightness(1); /* Brightens on hover */
    transform: translateY(-3px); /* Lifts the folder */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Pop-out shadow on hover */
}

/* Folder-specific fixed gradient backgrounds for TOP-LEVEL folders */
/* These rules now directly apply the background to the top-level folders. */

.nav-files-container > div > .nav-folder:nth-child(11n + 2) {
    background: linear-gradient(90deg, rgb(255, 180, 200), rgb(243, 139, 168), rgb(220, 100, 140));
}

.nav-files-container > div > .nav-folder:nth-child(11n + 3) {
    background: linear-gradient(90deg, rgb(255, 190, 200), rgb(235, 160, 172), rgb(210, 120, 140));
}

.nav-files-container > div > .nav-folder:nth-child(11n + 4) {
    background: linear-gradient(90deg, rgb(255, 210, 170), rgb(250, 179, 135), rgb(230, 140, 100));
}

.nav-files-container > div > .nav-folder:nth-child(11n + 5) {
    background: linear-gradient(90deg, rgb(255, 245, 210), rgb(249, 226, 175), rgb(220, 190, 130));
}

.nav-files-container > div > .nav-folder:nth-child(11n + 6) {
    background: linear-gradient(90deg, rgb(200, 250, 190), rgb(166, 227, 161), rgb(130, 190, 130));
}

.nav-files-container > div > .nav-folder:nth-child(11n + 7) {
    background: linear-gradient(90deg, rgb(180, 250, 240), rgb(148, 226, 213), rgb(110, 190, 180));
}

.nav-files-container > div > .nav-folder:nth-child(11n + 8) {
    background: linear-gradient(90deg, rgb(170, 240, 250), rgb(137, 220, 235), rgb(100, 180, 200));
}

.nav-files-container > div > .nav-folder:nth-child(11n + 9) {
    background: linear-gradient(90deg, rgb(150, 220, 250), rgb(116, 199, 236), rgb(80, 160, 200));
}

.nav-files-container > div > .nav-folder:nth-child(11n + 10) {
    background: linear-gradient(90deg, rgb(170, 200, 255), rgb(135, 176, 249), rgb(100, 140, 210));
}

.nav-files-container > div > .nav-folder:nth-child(11n + 11) {
    background: linear-gradient(90deg, rgb(210, 220, 255), rgb(180, 190, 254), rgb(140, 150, 220));
}

.nav-files-container > div > .nav-folder:nth-child(11n + 12) {
    background: linear-gradient(90deg, rgb(230, 200, 255), rgb(203, 166, 247), rgb(160, 120, 210));
}


/* Bold folder names (applies to text within any .nav-folder) */
.nav-files-container .nav-folder-title .nav-file-title-content,
.nav-files-container .nav-folder-title .nav-folder-title-content {
    font-weight: 500 !important;
    position: relative;
    z-index: 2;
    color: var(--nav-item-color) !important;
    text-shadow: none !important;
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

/* --- CRITICAL FIX: Make Subfolders Transparent --- */
/* This rule targets *any* subfolder and explicitly removes its background. */
.nav-files-container .nav-folder-children .nav-folder {
    background: transparent !important; /* Make background fully transparent */
    filter: none !important; /* Ensure no brightness/filter is applied */
    box-shadow: none !important; /* Remove any shadow from transparent subfolders */
    border: none !important; /* Remove any border from transparent subfolders */
}


/* Highlight for File Names on Hover */
.nav-files-container .nav-file:hover .nav-file-title-content {
    background-color: rgba(0, 0, 0, 0.1);
    border-radius: 4px;
    padding: 0 4px;
    margin: 0 -4px;
}

/* Ensure folder names do NOT get highlighted */
.nav-files-container .nav-folder-title:hover .nav-folder-title-content {
    background-color: transparent !important;
}

/* AnuPpuccin theme specific overrides (if necessary, keep these at the end) */
.theme-anupucin .nav-files-container .nav-folder-title .nav-file-title-content,
.theme-anupucin .nav-files-container .nav-folder-title .nav-folder-title-content {
    font-family: 'Inter', 'Segoe UI', system-ui, -apple-system, BlinkMacSystemFont, sans-serif !important;
}

📅 Interactive Calendar Animations Snippet
/* --- Calendar Day Lift Effect on Hover --- */

/* Base style for all calendar day elements */
/* This targets the main date cell, including the Svelte-generated hash for high specificity. */
div.day.svelte-q3wqg9 {
    position: relative; /* Essential for z-index and box-shadow positioning */
    /* Define transitions for smooth animation of transform, box-shadow, background, and color */
    transition: 
        transform 0.2s ease-out, /* Controls the lift and scale speed */
        box-shadow 0.2s ease-out, /* Controls the shadow appearance speed */
        background-color 0.1s ease-in, /* Preserves existing background color transition */
        color 0.1s ease-in; /* Preserves existing text color transition */
    z-index: 1; /* Default stacking order for non-hovered days */
}

/* Hover effect for all calendar day elements */
/* When the mouse hovers over a day, it lifts, scales slightly, and gets a shadow */
div.day.svelte-q3wqg9:hover {
    transform: translateY(-5px) scale(1.02); /* Lifts the element up by 5px and scales it to 102% */
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3); /* Adds a shadow for depth (adjust color/blur as needed) */
    z-index: 10; /* Brings the hovered day to the front, preventing overlap issues with shadows */
}

/* Reset z-index for non-hovered days */
/* Ensures that days return to their normal stacking order when the mouse moves away */
div.day.svelte-q3wqg9:not(:hover) {
    z-index: 1; 
}


/* --- Dynamic Dot Pulse Animation --- */

/* 1. Define the Keyframes Animation for a single dot pulse */
/* This animation describes one cycle of a dot expanding and contracting */
@keyframes dot-pulse {
    0% {
        transform: scale(1); /* Start at normal size */
        opacity: 0.8; /* Start slightly transparent */
    }
    50% {
        transform: scale(1.6); /* Expand to 160% of original size */
        opacity: 1; /* Become fully opaque */
    }
    100% {
        transform: scale(1); /* Return to normal size */
        opacity: 0.8; /* Return to slightly transparent */
    }
}

/* 2. Apply the animation to the FILLED dots when the PARENT DAY is hovered */
/* This targets only the 'filled' dots within the 'dot-container' when the main day is hovered. */
/* The Svelte hash (`.svelte-1widvzq`) is crucial for targeting these specific SVG elements. */
div.day.svelte-q3wqg9:hover .dot-container svg.dot.filled.svelte-1widvzq {
    /* Apply the defined 'dot-pulse' animation */
    animation: dot-pulse 1s infinite ease-in-out; /* 1s duration, repeats infinitely, smooth timing */
    
    /* Ensure the dot is visible and scaling from its center */
    opacity: 0.8; 
    transform-origin: center center;
}

/* 3. Stagger the animation using :nth-child() */
/* This creates the "quick succession" or "wave" effect for multiple dots. */
/* Adjust 'animation-delay' values to control the speed of the wave. */
/* Extended to cover up to 10 dots for broader compatibility. */

div.day.svelte-q3wqg9:hover .dot-container svg.dot.filled.svelte-1widvzq:nth-child(1) {
    animation-delay: 0s;
}
div.day.svelte-q3wqg9:hover .dot-container svg.dot.filled.svelte-1widvzq:nth-child(2) {
    animation-delay: 0.10s; /* Slightly faster delay for more dots */
}
div.day.svelte-q3wqg9:hover .dot-container svg.dot.filled.svelte-1widvzq:nth-child(3) {
    animation-delay: 0.20s;
}
div.day.svelte-q3wqg9:hover .dot-container svg.dot.filled.svelte-1widvzq:nth-child(4) {
    animation-delay: 0.30s;
}
div.day.svelte-q3wqg9:hover .dot-container svg.dot.filled.svelte-1widvzq:nth-child(5) {
    animation-delay: 0.40s;
}
div.day.svelte-q3wqg9:hover .dot-container svg.dot.filled.svelte-1widvzq:nth-child(6) {
    animation-delay: 0.50s;
}
div.day.svelte-q3wqg9:hover .dot-container svg.dot.filled.svelte-1widvzq:nth-child(7) {
    animation-delay: 0.60s;
}
div.day.svelte-q3wqg9:hover .dot-container svg.dot.filled.svelte-1widvzq:nth-child(8) {
    animation-delay: 0.70s;
}
div.day.svelte-q3wqg9:hover .dot-container svg.dot.filled.svelte-1widvzq:nth-child(9) {
    animation-delay: 0.80s;
}
div.day.svelte-q3wqg9:hover .dot-container svg.dot.filled.svelte-1widvzq:nth-child(10) {
    animation-delay: 0.90s;
}


/* Optional: Ensure dots are not animating by default (only on hover) */
/* This rule explicitly ensures no animation is applied when the day is not hovered. */
.dot-container svg.dot.filled.svelte-1widvzq {
    animation: none; 
}

/* Note on Hollow Dots: */
/* The `hollow` dot (if present, usually the last one) is excluded from the `dot-pulse`
   animation by targeting `svg.dot.filled`. If you wish to animate the hollow dot
   differently, you would create a separate `@keyframes` and apply it to 
   `div.day.svelte-q3wqg9:hover .dot-container svg.hollow.task.svelte-1widvzq`. */


⚙️ Customization
📁 Enhanced Folder & File Styling Customization
Folder Colors: Modify the rgb() values for --folder-color, --folder-color-light, and --folder-color-dark in each nth-child block to change the color palette of your folders.

Animation Speed (Animated Gradient): Adjust the 7s value in animation: rainbow-gradient-shift 7s ease-in-out infinite; to make the gradient animation faster or slower.

Hover Effect Intensity:

Change transform: translateY(-3px); to a different pixel value for more or less lift.

Adjust box-shadow values (0 6px 15px rgba(0, 0, 0, 0.1)) for a softer or stronger shadow.

Modify filter: brightness(1); on hover to make the folder brighter or darker.

Subfolder Gray Shade: Change the rgba(0, 0, 0, 0.8) value in the .nav-files-container .nav-folder-children .nav-folder-title .nav-folder-title-content rule to make subfolder text lighter or darker.

File Highlight: Adjust rgba(0, 0, 0, 0.1) in .nav-files-container .nav-file:hover .nav-file-title-content for a more or less opaque file highlight.

📅 Interactive Calendar Animations Customization
Date Lift Effect (div.day.svelte-q3wqg9:hover):

transform: translateY(-5px) scale(1.02);:

translateY(-5px): Controls how high the date lifts. Increase/decrease the px value.

scale(1.02): Controls how much the date slightly enlarges. Increase/decrease the value (e.g., 1.05 for a bigger effect).

box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);:

0 8px 16px: Adjust horizontal offset, vertical offset, and blur radius of the shadow.

rgba(0, 0, 0, 0.3): Change the color (first three numbers for RGB) and opacity (last number, 0 to 1) of the shadow.

transition duration: Adjust 0.2s for transform and box-shadow to make the lift faster or slower.

Dot Pulse Animation (@keyframes dot-pulse and animation properties):

@keyframes dot-pulse:

transform: scale(1.6); (at 50%): Controls how large the dot gets during its pulse.

opacity: 0.8; (at 0% and 100%): Controls the base transparency of the dots when not at their peak.

animation: dot-pulse 1s infinite ease-in-out;:

1s: The duration of one complete pulse cycle for a single dot. Make it shorter for a faster pulse, longer for a slower one.

ease-in-out: You can experiment with other timing functions like linear, ease, ease-in, ease-out for different feels.

animation-delay (:nth-child rules):

0.10s: This value determines the delay between each dot's pulse. A smaller value (e.g., 0.05s) will make the wave faster and tighter; a larger value will make it slower and more spread out.

The provided snippet now includes rules for up to 10 dots. If you consistently have more than 10 dots, you would need to add more :nth-child rules. For a truly dynamic number of dots beyond a reasonable CSS limit, a small JavaScript snippet would be required, but this goes beyond a pure CSS solution.
