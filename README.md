# Widget Testing Sandbox

This is a sandbox website designed for testing your before/after widget integration. It simulates a real beauty salon website where you can test how your widget looks and behaves in a realistic environment.

## Getting Started

1. **Open the website**: Simply open `index.html` in your web browser
2. **Navigate to the testing area**: Scroll down to the "Widget Testing Area" section
3. **Test your widget**: Use the provided integration points to test your widget

## Widget Integration Points

The sandbox provides three different integration points for testing:

### 1. Widget Integration Point 1
- **Location**: Main testing area
- **Purpose**: Primary widget placement testing
- **Container ID**: `widget-container-1`

### 2. Widget Integration Point 2
- **Location**: Alternative placement area
- **Purpose**: Testing different layouts and positioning
- **Container ID**: `widget-container-2`

### 3. Widget Integration Point 3 (Inline)
- **Location**: Embedded within content flow
- **Purpose**: Testing widget integration within existing content
- **Container ID**: `widget-container-3`

## How to Integrate Your Widget

### Production Widget Integration (Ready to Use!)

The sandbox now includes **production-ready before/after widgets** that you can test immediately:

#### Shadow DOM Variant (Default - Best Performance)
```html
<script async src="https://before-after-embed.vercel.app/embed.js"
    data-embed-id="bojo"
    data-theme="auto"
    data-max-width="400px"
    data-align="center">
</script>
```

#### Card Variant (Iframe - CSP Compatible)
```html
<script async src="https://before-after-embed.vercel.app/embed.js"
    data-embed-id="bojo"
    data-variant="card"
    data-theme="auto"
    data-max-width="500px"
    data-align="center">
</script>
```

### Method 1: Direct HTML Integration
Replace the placeholder content in any widget container with your widget code:

```html
<!-- Replace this placeholder -->
<div class="widget-placeholder">
    <h3>Widget Integration Point</h3>
    <!-- ... placeholder content ... -->
</div>

<!-- With your widget code -->
<div id="your-widget-container"></div>
<script src="your-widget.js"></script>
```

### Method 2: JavaScript Integration
Use the provided JavaScript functions to dynamically load your widget:

```javascript
// Load your widget into a container
function loadMyWidget(containerId) {
    const container = document.getElementById(containerId);
    container.innerHTML = `
        <div id="my-widget"></div>
        <script src="path/to/your-widget.js"></script>
    `;
}

// Call the function
loadMyWidget('widget-container-1');
```

## Testing Features

### Built-in Testing Tools
- **Simulate Widget Load**: Test button that simulates widget loading
- **Clear Widget**: Reset button to clear the widget and return to placeholder
- **Responsive Design**: Test how your widget behaves on different screen sizes

### Testing Scenarios
1. **Visual Integration**: See how your widget looks within the website's design
2. **Responsive Behavior**: Test widget behavior on mobile and desktop
3. **Content Flow**: Ensure your widget doesn't break the page layout
4. **Performance**: Monitor how your widget affects page load times

## Website Features

The sandbox includes:
- **Realistic Content**: Beauty salon theme with services, pricing, and contact info
- **Modern Design**: Professional styling with gradients, shadows, and animations
- **Responsive Layout**: Mobile-friendly design that adapts to different screen sizes
- **Interactive Elements**: Navigation, buttons, and hover effects
- **Multiple Sections**: Header, hero, services, widget testing area, and footer

## Customization

### Styling Your Widget
The sandbox provides CSS classes you can use or override:

```css
.widget-container {
    /* Main widget container styling */
    background: white;
    padding: 2rem;
    border-radius: 15px;
    box-shadow: 0 5px 20px rgba(0,0,0,0.1);
    margin: 2rem 0;
    min-height: 400px;
    border: 2px dashed #667eea;
}
```

### Color Scheme
- **Primary**: #667eea (Blue gradient)
- **Secondary**: #ff6b6b (Red accent)
- **Background**: #f8f9fa (Light gray)
- **Text**: #333 (Dark gray)

## Browser Compatibility

Test your widget across different browsers:
- Chrome (recommended for development)
- Firefox
- Safari
- Edge

## Performance Testing

Monitor these metrics when testing your widget:
- **Load Time**: How quickly your widget initializes
- **Memory Usage**: Impact on browser memory
- **CPU Usage**: Effect on page performance
- **Network Requests**: API calls and resource loading

## Troubleshooting

### Common Issues
1. **Widget not loading**: Check console for JavaScript errors
2. **Styling conflicts**: Use CSS specificity or !important declarations
3. **Responsive issues**: Test on different screen sizes
4. **Performance problems**: Optimize images and scripts

### Debug Tools
- **Browser DevTools**: Use F12 to inspect elements and debug
- **Console Logging**: Add console.log statements to track widget behavior
- **Network Tab**: Monitor API calls and resource loading

## Next Steps

1. **Test your widget** in all three integration points
2. **Verify responsive behavior** on mobile and desktop
3. **Check performance** impact on page load
4. **Validate accessibility** with screen readers
5. **Test cross-browser compatibility**

## Support

For widget integration issues:
1. Check browser console for errors
2. Verify widget script paths are correct
3. Ensure all dependencies are loaded
4. Test in incognito/private browsing mode

---

**Happy Testing!** 🎉

This sandbox is designed to help you create the best possible widget integration experience for your customers.
