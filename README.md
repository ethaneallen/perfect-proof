# Perfect Proof 🥃

A beautiful, fast whiskey dilution calculator for achieving your perfect pour. Calculate exactly how much water to add to any whiskey to reach your desired proof.

<img width="383" height="975" alt="image" src="https://github.com/user-attachments/assets/1b5a3128-f75a-45c6-b83f-10684ec5db55" />

## Features

🧮 **Precise Calculations**
- Calculates water needed to dilute whiskey to target proof
- Supports both U.S. proof and alcohol by volume (ABV)
- Real-time ABV display as you adjust values
- Shows final volume and proof

🌡️ **Flexible Units**
- Seamlessly convert between fluid ounces (fl. oz.) and milliliters (ml)
- Switch units for input whiskey amount
- Switch units for calculated water amount
- Your preferred units are saved for next session

🎨 **Beautiful UI**
- Modern dark mode (default) and light mode
- Smooth animations and transitions
- Responsive design - works on desktop, tablet, and mobile
- Visual ratio bar showing whiskey-to-water proportion
- Built with Tailwind CSS and optimized for all screen sizes

⚡ **Quick Presets**
- One-click preset buttons for common proof levels
- Popular whiskey proofs: 100, 110, 120, 127
- Common dilution targets: 80, 90, 95, 100
- Instantly calculate when you select a preset

💾 **Smart Preferences**
- Saves your calculations and preferences locally
- Theme preference (dark/light mode)
- Preferred units (fl. oz. or ml)
- Last used values for quick repeating calculations

📋 **Share Results**
- Copy calculation results to clipboard
- Formatted recipe-style output
- Great for sharing with friends or recording notes

## How to Use

1. **Enter Whiskey Amount**: Input how much whiskey you're starting with
   - Toggle between fl. oz. and ml as needed

2. **Set Bottle Proof**: Enter the proof level of your whiskey
   - Use preset buttons for common proofs (100, 110, 120, 127)
   - ABV is displayed automatically

3. **Choose Desired Proof**: What proof do you want to achieve?
   - Use preset buttons or enter your own value
   - Desired proof must be lower than bottle proof

4. **Calculate**: Click "Calculate Water Needed" (or press Enter)
   - See exactly how much water to add
   - View the final volume and proof
   - Check the whiskey-to-water ratio

5. **Copy & Share**: Click "Copy Result" to save to clipboard

## Proof & ABV Reference

**Understanding Proof:**
- Proof = ABV × 2
- A 100 proof whiskey = 50% ABV
- A standard bottle (750ml) of 80 proof whiskey = 40% ABV

**Common Whiskey Proofs:**
- **80 proof** - Standard commercial whiskey (40% ABV)
- **90 proof** - Regular bottle strength (45% ABV)
- **100 proof** - Bottled-in-bond standard (50% ABV)
- **110 proof** - High rye bourbon (55% ABV)
- **120 proof** - Barrel proof range (60% ABV)
- **127 proof** - Premium barrel proof (63.5% ABV)

## Installation

### Option 1: Direct Use
Simply open `perfect-proof.html` in any modern web browser.

### Option 2: Host Locally
Copy the HTML file to your web server:

```bash
# With Python 3
python -m http.server 8000

# With Node.js
npx serve
```

Then navigate to `http://localhost:8000`

## Technologies

- **HTML5** - Semantic markup
- **Tailwind CSS** - Modern responsive styling
- **Vanilla JavaScript** - No dependencies, pure calculations
- **localStorage** - Persistent preference storage

## Browser Compatibility

Works on all modern browsers:
- ✅ Chrome/Edge 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## File Structure

```
perfect-proof/
├── perfect-proof.html    # Complete application (single file)
└── README.md             # This file
```

## Customization

To customize colors and styling, edit the CSS variables in the `<style>` section:

```css
:root {
    --bg-primary: #f8fafc;      /* Background color */
    --bg-card: linear-gradient(...);  /* Card background */
    --text-primary: #ffffff;    /* Primary text */
    --text-secondary: #9ca3af;  /* Secondary text */
    --border-color: rgba(...);  /* Border color */
}
```

Toggle light mode support by modifying the `body.light-mode` CSS rules.

## Formula

The calculator uses the standard dilution formula:

```
Water Volume = Whiskey Volume × ((Bottle Proof / Desired Proof) - 1)
```

This ensures the final mixture reaches your target proof while accounting for volume additivity.

## Tips for Perfect Results

1. **Chill Everything**: Add water to slightly chilled whiskey for the best integration
2. **Use Quality Water**: Filtered or distilled water produces better results than tap water
3. **Let It Rest**: After dilution, let your pour rest for 30 seconds to allow the flavors to open
4. **Temperature Matters**: Room temperature is ideal for nosing and tasting
5. **Hard Water**: Mineral content can affect taste - use filtered water for consistency

## Common Dilution Ratios

| Bottle Proof | Desired Proof | Ratio |
|-------------|--------------|-------|
| 100         | 80           | 4:1 (whiskey:water) |
| 110         | 90           | 4.7:1 |
| 120         | 100          | 5:1   |
| 127         | 95           | 5.7:1 |

## License

MIT License - Feel free to use, modify, and distribute this project.

## Contributing

Contributions welcome! Feel free to submit a Pull Request with improvements or bug fixes.

## Acknowledgments

Built for whiskey enthusiasts who appreciate precision mixing and perfect pours. Inspired by classic dilution practices and modern mixing science. 🥃

---

Perfect Proof Calculator - Made for the spirit of precision.
