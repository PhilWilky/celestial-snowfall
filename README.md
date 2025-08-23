# ❄️ Celestial Snowfall

A beautiful, interactive winter night sky scene with falling snow, twinkling stars, shooting stars, and a glowing moon. Perfect for adding magical Christmas atmosphere to any website during the festive season.

## ✨ Features

- **Realistic snowfall** with depth-based physics and wind effects
- **Twinkling starfield** with randomized positions and brightness
- **Dynamic shooting stars** with multiple realistic trajectories
- **Glowing moon** with subtle crater details
- **Interactive controls** for pause/resume and snow density
- **Accessibility friendly** with reduced motion support
- **Mobile optimized** with performance considerations
- **Zero dependencies** - pure vanilla JavaScript and CSS

## 🎥 Demo

[Live Demo](https://philwilky.github.io/celestial-snowfall/)

## 🚀 Quick Start

### Standalone Version
Simply download `night-sky-standalone.html` and open it in your browser. That's it! 

### Website Overlay Version
Perfect for adding Christmas magic to existing websites:

```html
<!-- Add this CSS to your <head> -->
<link rel="stylesheet" href="night-sky-overlay.css">

<!-- Add this div anywhere in your <body> -->
<div class="night-sky-overlay" id="nightSkyOverlay">
  <!-- Overlay content will be inserted here -->
</div>

<!-- Add this script before closing </body> -->
<script src="night-sky-overlay.js"></script>
```

## 🎛️ Controls

- **Pause/Resume Button** - Stop or start all animations
- **Density Slider** - Control snowfall intensity (1 = light snow, 10 = blizzard)

## 🎨 Customization

The night sky is highly customizable through CSS variables and JavaScript configuration:

### CSS Variables
```css
:root {
  --star-count: 80;                    /* Number of stars */
  --snow-density: 5;                   /* Default snow density */
  --shooting-star-interval-min: 4000;  /* Min time between shooting stars (ms) */
  --shooting-star-interval-max: 10000; /* Max time between shooting stars (ms) */
}
```

### Color Themes
Easily change the color scheme by modifying the CSS:
```css
/* Change snow color */
.snowflake path { stroke: #your-color; }
.snowflake circle { fill: #your-color; }

/* Change star color */
.star { 
  background: #your-color;
  box-shadow: 0 0 8px #your-glow-color;
}

/* Change background gradient */
body {
  background: radial-gradient(/* your custom gradient */);
}
```

## 📱 Browser Support

- ✅ Modern Chrome, Firefox, Safari, Edge
- ✅ Mobile browsers (with automatic performance optimization)
- ⚠️ IE11+ (limited support, some features may not work)

## ♿ Accessibility

- Respects `prefers-reduced-motion` setting
- Animations automatically pause for users with motion sensitivity
- All decorative elements are properly marked with `aria-hidden="true"`
- Keyboard accessible controls

## 🔧 Technical Details

### Performance Optimizations
- **Hardware acceleration** using `will-change` and `transform3d`
- **Automatic cleanup** of DOM elements to prevent memory leaks  
- **Mobile detection** with reduced particle counts
- **Efficient animation** using Web Animations API and CSS transitions

### Architecture
- **Modular design** with separate managers for stars, snow, and shooting stars
- **Self-contained** JavaScript with no global pollution
- **Namespaced CSS** to prevent conflicts with existing styles

## 📦 File Structure

```
celestial-snowfall/
├── README.md
├── LICENSE
├── night-sky-standalone.html      # Complete standalone version
├── night-sky-overlay.html         # Website integration demo
├── dist/
│   ├── night-sky-overlay.css      # Overlay styles only
│   ├── night-sky-overlay.js       # Overlay script only
│   └── night-sky-overlay.html     # HTML snippet for integration
└── examples/
    ├── wordpress-integration.php
    ├── react-wrapper.jsx
    └── simple-integration.html
```

## 🎄 Use Cases

Perfect for:
- **Christmas landing pages** and festive websites
- **Christmas e-commerce** stores and seasonal promotions  
- **Christmas events** and winter celebrations
- **Ambient backgrounds** for holiday presentations or demos
- **Creative portfolios** showcasing Christmas animation skills
- **Educational projects** demonstrating CSS/JS animation techniques during the holiday season

## 🛠️ Development

Want to contribute or modify the code?

1. Clone the repository:
   ```bash
   git clone https://github.com/PhilWilky/celestial-snowfall.git
   cd celestial-snowfall
   ```

2. Open `night-sky-standalone.html` in your browser

3. Make your changes and test across different browsers

4. Submit a pull request with your improvements!

### Development Tips
- Use browser dev tools to adjust timing and physics
- Test on both desktop and mobile devices
- Check performance with many particles active
- Verify accessibility with screen readers

## 🤝 Contributing

Contributions are welcome! Here are some ideas:

- 🌈 **New themes** (aurora borealis, autumn leaves, spring rain)
- 🎵 **Sound effects** (optional wind, snow sounds)
- 🎮 **Interactive elements** (click to create shooting stars)
- 🌍 **Internationalization** (multiple language support)
- 📱 **PWA features** (offline support, app-like installation)
- ⚡ **Performance improvements** (WebGL rendering, worker threads)

Please read the [contribution guidelines](CONTRIBUTING.md) before submitting PRs.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

You're free to use this in personal and commercial projects. Just keep the copyright notice intact!

## 🙏 Acknowledgments

- Inspired by real winter nights and childhood snow days
- Built with love for the web development community
- Special thanks to everyone who provides feedback and contributions

## 🔗 Links

- [Issues](https://github.com/PhilWilky/celestial-snowfall/issues) - Report bugs or request features

---

**Made with ❄️ and Christmas spirit by [Philip "Phil" Wilkinson](https://github.com/PhilWilky)**

*If you find this useful, consider giving it a ⭐ star on GitHub!*