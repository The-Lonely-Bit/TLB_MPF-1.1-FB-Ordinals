# Customizing Your Collection's Design

## Introduction

The `design.json` file allows you to customize the appearance of your collection’s minting page on **TLB MintPumpFun**. You can modify elements such as background images, text colors, fonts, button styles, and more.

### Default Design Template
The default `design.json` file looks like this:

```json
{
  "global": {
    "background": "url('collections/TLB_010/background.png') no-repeat center center fixed",
    "text-color": "#ffcc00",
    "font-family": "'Roboto', sans-serif",
    "logo-filter": "drop-shadow(0 0 4px rgba(0,0,0,0.5))",
    "header-bg": "rgb(134 134 134 / 95%)",
    "nav-link-color": "#003366",
    "nav-link-hover": "#ffcc00",
    "button-bg": "#ffcc00",
    "button-color": "#003366",
    "matrix-text-color": "#ffcc00",
    "card-border-color": "#ffcc00",
    "modal-background": "rgba(255,255,255,0.95)",
    "scanline-color": "transparent",
    "filter-select-bg": "#ffffff",
    "price-input-bg": "#ffffff",
    "item-card-bg": "#003366",
    "item-card-border": "1px solid #ffcc00"
  },
  "selectors": {
    "html, body": {
      "margin": "0",
      "padding": "0",
      "overflow-x": "hidden",
      "height": "100%",
      "background-size": "cover"
    }
  },
  "matrixEnabled": false
}
```

---

## How to Modify Your Collection's Design

You can edit the `design.json` file to customize the look and feel of your minting page. Below is a breakdown of what each section does and how you can modify it.

### 1. **Global Styles**
The `global` section defines general appearance settings. You can modify the following properties:

| Property            | Description | Example |
|--------------------|-------------|---------|
| `background`       | Sets the background image or color | `"#000000"` or `"url('collections/my_collection/bg.png') no-repeat center center fixed"` |
| `text-color`       | Defines the main text color | `"#ffffff"` |
| `font-family`      | Sets the font style | `"'Arial', sans-serif"` |
| `logo-filter`      | Adds effects to the logo | `"drop-shadow(0 0 5px rgba(255, 255, 255, 0.5))"` |
| `header-bg`        | Background color of the header | `"rgba(0,0,0,0.8)"` |
| `nav-link-color`   | Navigation link text color | `"#ffcc00"` |
| `nav-link-hover`   | Navigation link hover color | `"#ff6600"` |
| `button-bg`        | Background color of buttons | `"#ffcc00"` |
| `button-color`     | Button text color | `"#000000"` |
| `matrix-text-color`| Text color in Matrix effect | `"#0f0"` |
| `card-border-color`| NFT item card border color | `"#ffcc00"` |
| `modal-background` | Background color of pop-ups | `"rgba(0,0,0,0.9)"` |
| `scanline-color`   | Scanline effect color | `"transparent"` |
| `filter-select-bg` | Background of dropdowns and filters | `"#222222"` |
| `price-input-bg`   | Background color for price input fields | `"#ffffff"` |
| `item-card-bg`     | Background color of NFT cards | `"#333333"` |
| `item-card-border` | Border style for NFT cards | `"1px solid #ffcc00"` |

---

### 2. **CSS Selectors**
The `selectors` section lets you apply custom styles to specific elements of your page. You can modify spacing, layout, and other CSS properties.

For example, to change the page margins and prevent horizontal scrolling:

```json
"html, body": {
  "margin": "0",
  "padding": "0",
  "overflow-x": "hidden",
  "height": "100%",
  "background-size": "cover"
}
```

You can add more styles to customize elements further, such as:

```json
".item-card": {
  "border-radius": "10px",
  "box-shadow": "0 0 10px rgba(255, 255, 255, 0.3)"
}
```

---

### 3. **Enabling or Disabling the Matrix Effect**

The **Matrix effect** adds a cyberpunk-style animated text overlay. By default, this effect is disabled.

To enable it, set:

```json
"matrixEnabled": true
```

To disable it:

```json
"matrixEnabled": false
```

---

## How to Apply Your Custom Design

1. Open the `design.json` file in a text editor.
2. Modify the values according to your preferences.
3. Save the file and upload it to your collection’s directory (e.g., `collections/my_collection/design.json`).
4. Refresh your minting page to see the changes.

---

## Need Help?
If you need assistance customizing your design, feel free to reach out to the **TLB MintPumpFun** community for support.

🚀 **Take full control of your minting page and make it truly yours!**
