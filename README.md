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

Flatcap draws inspiration from the fantastic design logic of the **[Nord theme](https://github.com/nordtheme/nord)**, embracing its principles of calm, clean aesthetics, and a dimmed pastel color approach. This results in a theme that is both familiar in its minimalist comfort and fresh in its distinct, modern color scheme.

## Color Palette

The Flatcap theme is built upon a carefully curated and expanded color palette, designed for granular control and visual harmony across various UI elements and syntax highlighting. The palette is divided into four main categories: Deep Twilight, Dawnlight, Ocean Blues, and Vivid Accents.

### Deep Twilight (Dark Backgrounds & Base Elements)

<p>
  <img src="https://placehold.co/100x100/1c1e22/6b7f8e/png?font=source-sans-pro&text=%231c1e22" />
  <img src="https://placehold.co/100x100/23262b/6b7f8e/png?font=source-sans-pro&text=%2323262b" />
  <img src="https://placehold.co/100x100/2d3036/6b7f8e/png?font=source-sans-pro&text=%232d3036" />
  <img src="https://placehold.co/100x100/373a40/6b7f8e/png?font=source-sans-pro&text=%23373a40" />
  <img src="https://placehold.co/100x100/42474e/6b7f8e/png?font=source-sans-pro&text=%2342474e" />
</p>

These colors are primarily used for backgrounds, elevated UI elements, and low-priority components in dark ambiance designs.

- **Flatcap 0**: `#1c1e22` - Interface base, the darkest tone.
- **Flatcap 1**: `#23262b` - Secondary panel backgrounds, subtle UI elements.
- **Flatcap 2**: `#2d3036` - Elevated UI element backgrounds, active editor lines, containers.
- **Flatcap 3**: `#373a40` - Borders, separators, code comments, secondary text.
- **Flatcap 4**: `#42474e` - Subtle shadows, semi-transparent overlays, highly muted text.

### Dawnlight (Light Text & UI Elements)

<p>
  <img src="https://placehold.co/100x100/b0b4ba/6b7f8e/png?font=source-sans-pro&text=%231c1e22" />
  <img src="https://placehold.co/100x100/c8ccda/6b7f8e/png?font=source-sans-pro&text=%231c1e22" />
  <img src="https://placehold.co/100x100/dce0eb/6b7f8e/png?font=source-sans-pro&text=%231c1e22" />
  <img src="https://placehold.co/100x100/eef1f6/6b7f8e/png?font=source-sans-pro&text=%231c1e22" />
  <img src="https://placehold.co/100x100/f6f8fa/6b7f8e/png?font=source-sans-pro&text=%231c1e22" />
</p>

Perfect for main text, contrasting UI elements, and light backgrounds.

- **Flatcap 5**: `#b0b4ba` - Low-contrast text in dark mode, main text in light mode.
- **Flatcap 6**: `#c8ccda` - Main text in dark mode, clear UI elements.
- **Flatcap 7**: `#dce0eb` - Light container backgrounds, interactive UI elements.
- **Flatcap 8**: `#eef1f6` - Brightest tone for light base backgrounds, maximum highlights.
- **Flatcap 9**: `#f6f8fa` - Very specific elements requiring highest contrast or purity, like light mode selection highlights.

### Ocean Blues (Primary UI Components & Syntax)

<p>
  <img src="https://placehold.co/100x100/6b7f8e/42474e/png?font=source-sans-pro&text=%236b7f8e" />
  <img src="https://placehold.co/100x100/7a90a2/42474e/png?font=source-sans-pro&text=%237a90a2" />
  <img src="https://placehold.co/100x100/8ea5b9/42474e/png?font=source-sans-pro&text=%238ea5b9" />
  <img src="https://placehold.co/100x100/a3bbce/42474e/png?font=source-sans-pro&text=%23a3bbce" />
  <img src="https://placehold.co/100x100/b8d1e3/42474e/png?font=source-sans-pro&text=%23b8d1e3" />
</p>

The core of the palette, used for key UI components and code syntax, now with a more noticeable tonal progression.

- **Flatcap 10**: `#6b7f8e` - Darker grayish-blue, for less prominent syntax elements or informational UI.
- **Flatcap 11**: `#7a90a2` - Medium blue for classes and operators, primary buttons.
- **Flatcap 12**: `#8ea5b9` - Lighter and more distinctive blue for variables and selection highlights.
- **Flatcap 13**: `#a3bbce` - Bright blue for strings, numbers, or active links, enhancing visibility.
- **Flatcap 14**: `#b8d1e3` - Softer, ethereal blue, for decorative elements or very subtle colored backgrounds.

### Vivid Accents (States & Special Syntax)

<p>
  <img src="https://placehold.co/100x100/e06c75/42474e/png?font=source-sans-pro&text=%23e06c75" />
  <img src="https://placehold.co/100x100/d19a66/42474e/png?font=source-sans-pro&text=%23d19a66" />
  <img src="https://placehold.co/100x100/98c379/42474e/png?font=source-sans-pro&text=%2398c379" />
  <img src="https://placehold.co/100x100/c678dd/42474e/png?font=source-sans-pro&text=%23c678dd" />
  <img src="https://placehold.co/100x100/56b6c2/42474e/png?font=source-sans-pro&text=%2356b6c2" />
</p>

Used to indicate various states (error, warning, success) and to highlight specific syntax elements.

- **Flatcap 15**: `#e06c75` (Error) - Red for error messages.
- **Flatcap 16**: `#d19a66` (Warning) - Orange for warnings.
- **Flatcap 17**: `#98c379` (Success) - Green for success indications.
- **Flatcap 18**: `#c678dd` (Information) - Purple for informational messages.
- **Flatcap 19**: `#56b6c2` (Highlight) - Cyan for syntax highlighting, prominent visual accents.
