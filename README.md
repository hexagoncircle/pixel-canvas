# pixel-canvas

Web Component that applies a shimmering pixel background on element hover.

🖋️ Read the blog post: https://ryanmulligan.dev/blog/pixel-canvas/

## Usage

Include the component script and then insert a pixel-canvas custom element inside the container it should fill.

```html
<script type="module" src="pixel-canvas.js"></script>

<div class="container">
  <pixel-canvas></pixel-canvas>
  <!-- other elements -->
</div>
```

## Options

- `data-colors`: Comma-separated list of color values; i.e. `"#e0f2fe, #7dd3fc, #0ea5e9"`
- `data-gap`: Amount of space between each pixel. Accepts values between `4` and `50`.
- `data-speed`: Controls the general animation duration. Accepts values between `0` and `100`.
- `data-no-focus`: When any sibling element is focused, the animation plays. This disables the animation on focus events.

⚠️ If reduced motion preferences are set, the pixels all fade in at once (no stagger) and do not shimmer (speed is set to `0`).

Example with options:

```html
<div class="container">
  <pixel-canvas
    data-gap="10"
    data-speed="25"
    data-colors="#e0f2fe, #7dd3fc, #0ea5e9"
  ></pixel-canvas>
  <!-- other elements -->
</div>
```
