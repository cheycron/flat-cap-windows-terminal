<p align="center">
  <img src="https://github.com/cheycron/flat-cap-theme/blob/main/images/readme_logo.png?raw=true" alt="flatcap"/>
</p>

<p align="center">
  Flat Cap is a dark, minimalist, and eye-friendly theme meticulously crafted to provide a comfortable and focused experience.
</p>

[![BuyMeACoffee](https://raw.githubusercontent.com/pachadotdev/buymeacoffee-badges/main/bmc-blue.svg)](https://www.buymeacoffee.com/cheycron)

<p align="center">
  <img src="https://github.com/cheycron/flat-cap-theme/blob/main/images/demo_windowsterminal.png?raw=true" alt="Flatcap Windows Terminal"/>
</p>

## Installation

> [!WARNING]
> **Disclaimer:** Do not replace your entire `settings.json` file with the content of `app-windows-terminal.json`. Doing so will erase your existing profiles and settings. Instead, follow the steps below to add the color scheme manually.

1.  **Open Settings**: In Windows Terminal, open the **Settings** tab (you can use the `Ctrl + ,` shortcut). In the bottom-left corner, click on **Open JSON file**. This will open your `settings.json` file in your default text editor.

2.  **Add the Color Scheme**: In the `settings.json` file, find the `schemes` array. If it doesn't exist, you can add it. Copy the following JSON object and paste it inside the `schemes` array.

    ```json
    {
        "name": "Flat Cap",
        "background": "#1c1e22",
        "black": "#1c1e22",
        "blue": "#7a90a2",
        "brightBlack": "#42474e",
        "brightBlue": "#8ea5b9",
        "brightCyan": "#56b6c2",
        "brightGreen": "#98c379",
        "brightPurple": "#c678dd",
        "brightRed": "#e06c75",
        "brightWhite": "#fcfdff",
        "brightYellow": "#d19a66",
        "cursorColor": "#56b6c2",
        "cyan": "#a3bbce",
        "foreground": "#e4e6eb",
        "green": "#98c379",
        "purple": "#c678dd",
        "red": "#e06c75",
        "selectionBackground": "#2d3036",
        "white": "#e4e6eb",
        "yellow": "#d19a66"
    }
    ```

3.  **Apply the Theme**: Now, you need to apply this scheme to one of your profiles (like PowerShell, Command Prompt, or WSL).
    - Find the `profiles` object and then the `list` array inside it.
    - Choose the profile you want to change and add or modify the following line:
      ```json
      "colorScheme": "Flat Cap"
      ```
    - Alternatively, to apply it to **all** profiles, add this line to the `defaults` object within `profiles`:
      ```json
      "profiles": {
          "defaults": {
              "colorScheme": "Flat Cap"
          },
          "list": [ ... ]
      }
      ```

4.  **Save**: Save the `settings.json` file. Windows Terminal will automatically apply the changes.

## Philosophy

Flat Cap draws inspiration from the fantastic design logic of the **[Nord theme](https://github.com/nordtheme/nord)**, embracing its principles of calm, clean aesthetics, and a dimmed pastel color approach. However, Flat Cap diverges significantly in its color palette, which is uniquely derived from the visual language of the latest **Horizon OS** iterations by Meta for Oculus Quest. This fusion results in a theme that is both familiar in its minimalist comfort and fresh in its distinct, modern color scheme.

## Color Palette

The Flat Cap theme is built upon a carefully curated and expanded color palette, designed for granular control and visual harmony across various UI elements and syntax highlighting. The palette is divided into four main categories: Deep Twilight, Dawnlight, Ocean Blues, and Vivid Accents.

<p align="center">
  <img src="https://github.com/cheycron/flat-cap-theme/blob/main/images/color_deeptwilight.png?raw=true" alt="Deep Twilight"/>
</p>
<p align="center">
  <img src="https://github.com/cheycron/flat-cap-theme/blob/main/images/color_dawnlight.png?raw=true" alt="Dawnlight"/>
</p>
<p align="center">
  <img src="https://github.com/cheycron/flat-cap-theme/blob/main/images/color_oceanblues.png?raw=true" alt="Ocean Blues"/>
</p>
<p align="center">
  <img src="https://github.com/cheycron/flat-cap-theme/blob/main/images/color_vividaccents.png?raw=true" alt="Vivid Accents"/>
</p>

### Deep Twilight (Dark Backgrounds & Base Elements)

These colors are primarily used for backgrounds, elevated UI elements, and low-priority components in dark ambiance designs.

- **FlatCap 0**: `#1c1e22` - Interface base, the darkest tone.
- **FlatCap 1**: `#23262b` - Secondary panel backgrounds, subtle UI elements.
- **FlatCap 2**: `#2d3036` - Elevated UI element backgrounds, active editor lines, containers.
- **FlatCap 3**: `#373a40` - Borders, separators, code comments, secondary text.
- **FlatCap 4**: `#42474e` - Subtle shadows, semi-transparent overlays, highly muted text.

### Dawnlight (Light Text & UI Elements)

Perfect for main text, contrasting UI elements, and light backgrounds.

- **FlatCap 5**: `#d0d2d6` - Low-contrast text in dark mode, main text in light mode.
- **FlatCap 6**: `#e4e6eb` - Main text in dark mode, clear UI elements.
- **FlatCap 7**: `#ecedf0` - Light container backgrounds, interactive UI elements.
- **FlatCap 8**: `#f4f5f7` - Brightest tone for light base backgrounds, maximum highlights.
- **FlatCap 9**: `#fcfdff` - Very specific elements requiring highest contrast or purity, like light mode selection highlights.

### Ocean Blues (Primary UI Components & Syntax)

The core of the palette, used for key UI components and code syntax, now with a more noticeable tonal progression.

- **FlatCap 10**: `#6b7f8e` - Darker grayish-blue, for less prominent syntax elements or informational UI.
- **FlatCap 11**: `#7a90a2` - Medium blue for classes and operators, primary buttons.
- **FlatCap 12**: `#8ea5b9` - Lighter and more distinctive blue for variables and selection highlights.
- **FlatCap 13**: `#a3bbce` - Bright blue for strings, numbers, or active links, enhancing visibility.
- **FlatCap 14**: `#b8d1e3` - Softer, ethereal blue, for decorative elements or very subtle colored backgrounds.

### Vivid Accents (States & Special Syntax)

Used to indicate various states (error, warning, success) and to highlight specific syntax elements.

- **FlatCap 15**: `#e06c75` (Error) - Red for error messages.
- **FlatCap 16**: `#d19a66` (Warning) - Orange for warnings.
- **FlatCap 17**: `#98c379` (Success) - Green for success indications.
- **FlatCap 18**: `#c678dd` (Information) - Purple for informational messages.
- **FlatCap 19**: `#56b6c2` (Highlight) - Cyan for syntax highlighting, prominent visual accents.
