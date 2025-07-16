<p align="center">
  <img src="https://github.com/cheycron/flat-cap-theme/blob/main/images/readme_logo.png?raw=true" alt="flatcap"/>
</p>

<p align="center">
  Flat Cap is a dark, minimalist, and eye-friendly theme meticulously crafted to provide a comfortable and focused experience.
</p>

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
        "name": "Flatcap",
        "background": "#121418",
        "black": "#121418",
        "blue": "#81a1c1",
        "brightBlack": "#484f5c",
        "brightBlue": "#88c0d0",
        "brightCyan": "#00a8e0",
        "brightGreen": "#84dcc6",
        "brightPurple": "#81a1c1",
        "brightRed": "#ff70a6",
        "brightWhite": "#e4e6e9",
        "brightYellow": "#ffd670",
        "cursorColor": "#88c0d0",
        "cyan": "#8fbcbb",
        "foreground": "#cbced5",
        "green": "#84dcc6",
        "purple": "#5e81ac",
        "red": "#ff70a6",
        "selectionBackground": "#23272f",
        "white": "#cbced5",
        "yellow": "#ffd670"
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
  <img src="https://placehold.co/100x100/121418/5e81ac/png?font=source-sans-pro&text=%23121418" />
  <img src="https://placehold.co/100x100/191c22/5e81ac/png?font=source-sans-pro&text=%23191c22" />
  <img src="https://placehold.co/100x100/23272f/5e81ac/png?font=source-sans-pro&text=%2323272f" />
  <img src="https://placehold.co/100x100/303540/5e81ac/png?font=source-sans-pro&text=%23303540" />
  <img src="https://placehold.co/100x100/484f5c/5e81ac/png?font=source-sans-pro&text=%23484f5c" />
</p>

These colors form the foundational layers of a dark interface, creating a sense of depth and focus. They are ideal for establishing a clear visual hierarchy, from the main application window to interactive surfaces.

- **Flatcap 0**: `#121418` - **Main Background**: The deepest shade, perfect for the primary application background or the editor surface. It makes foreground elements stand out, reducing visual noise and helping the user focus on the content.
- **Flatcap 1**: `#191c22` - **Secondary Surfaces**: Slightly lighter, this color is ideal for secondary panels like sidebars, tree views, or inactive tabs. It subtly separates auxiliary sections from the main content area without creating a harsh contrast.
- **Flatcap 2**: `#23272f` - **Elevated Elements & Hover States**: Used for surfaces that appear "closer" to the user, such as modal dialogs, pop-up menus, or cards. It also works perfectly as a hover state for elements using Flatcap 1, providing clear interactive feedback.
- **Flatcap 3**: `#303540` - **Borders & Dividers**: The ideal choice for creating subtle separation. Use it for borders on panels, dividers in lists, or rulers in an editor. It's also excellent for secondary text, like code comments or placeholder hints in input fields, that should be present but not distracting.
- **Flatcap 4**: `#484f5c` - **Subtle Details & Disabled States**: Perfect for UI details that require minimal emphasis, such as subtle drop shadows, scrollbar tracks, or the background of a disabled button. It can also be used for highly muted, non-essential text.

### Dawnlight (Light Text & UI Elements)

<p>
  <img src="https://placehold.co/100x100/b2b6bf/5e81ac/png?font=source-sans-pro&text=%23b2b6bf" />
  <img src="https://placehold.co/100x100/bfc2ca/5e81ac/png?font=source-sans-pro&text=%23bfc2ca" />
  <img src="https://placehold.co/100x100/cbced5/5e81ac/png?font=source-sans-pro&text=%23cbced5" />
  <img src="https://placehold.co/100x100/d8dadf/5e81ac/png?font=source-sans-pro&text=%23d8dadf" />
  <img src="https://placehold.co/100x100/e4e6e9/5e81ac/png?font=source-sans-pro&text=%23e4e6e9" />
</p>

This group provides the clean, legible text and bright surfaces essential for a comfortable reading experience and a crisp, modern look in both dark and light themes. The tonal progression has been softened to offer a more delicate and refined contrast.

- **Flatcap 5**: `#b2b6bf` - **Low-Priority & Hint Text**: This darker, subtle shade is perfect for non-essential text like metadata, timestamps, or breadcrumbs. Its low contrast makes it ideal for information that should be available without drawing attention.
- **Flatcap 6**: `#bfc2ca` - **Secondary Text & Comments**: A medium-contrast color, excellent for secondary text, descriptions, or code comments. It's clearly legible but distinct from the main text, helping to establish an informational hierarchy.
- **Flatcap 7**: `#cbced5` - **Primary Text**: The standard for all primary body text in a dark interface. It offers exceptional readability against the Deep Twilight backgrounds without causing eye strain, striking a perfect balance between clarity and comfort.
- **Flatcap 8**: `#d8dadf` - **Highlight Text & Titles**: Used to give prominence to headings, titles, or active menu items. Its added brightness sets it apart as an element of higher importance. In a light theme, it serves as an excellent base background.
- **Flatcap 9**: `#e4e6e9` - **High-Impact Text & Focus Accents**: Reserved for the most important text elements or for the hover state on interactive text. Its maximum brightness ensures high visibility and can be used for high-contrast accents, like the fill of an active checkbox.

### Ocean Blues (Primary UI Components & Syntax)

<p>
  <img src="https://placehold.co/100x100/5e81ac/484f5c/png?font=source-sans-pro&text=%235e81ac" />
  <img src="https://placehold.co/100x100/81a1c1/484f5c/png?font=source-sans-pro&text=%2381a1c1" />
  <img src="https://placehold.co/100x100/88c0d0/484f5c/png?font=source-sans-pro&text=%2388c0d0" />
  <img src="https://placehold.co/100x100/8fbcbb/484f5c/png?font=source-sans-pro&text=%238fbcbb" />
  <img src="https://placehold.co/100x100/95b1b0/484f5c/png?font=source-sans-pro&text=%2395b1b0" />
</p>

This family of blues brings a calm yet confident energy to the interface. These colors are the primary actors, guiding the user's attention to interactive elements and making the UI feel responsive and intuitive.

- **Flatcap 10**: `#5e81ac` - **Subtle Actions & Informational Icons**: A darker, more reserved blue ideal for secondary buttons, informational icons, or unselected tabs. It indicates interactivity without demanding immediate attention.
- **Flatcap 11**: `#81a1c1` - **Primary Buttons & Links**: The quintessential color for primary actions. Use it for "Submit", "Save", or "Apply" buttons. It's also perfect for hyperlinks within text, providing a clear visual cue for navigation.
- **Flatcap 12**: `#88c0d0` - **Selection & Focus Highlights**: A brighter, more distinct blue perfect for highlighting selected items in a list, the active line in a code editor, or the border of a focused input field. It clearly communicates "what's currently active."
- **Flatcap 13**: `#8fbcbb` - **Active States & Progress Indicators**: This vibrant, almost turquoise blue is excellent for the active state of a toggle switch, a pressed button, or a progress bar. It draws the eye and confirms an action is underway or a state is "on."
- **Flatcap 14**: `#95b1b0` - **Decorative Accents & Subtle Backgrounds**: A soft, ethereal blue perfect for decorative elements like notification dots, subtle background highlights for the "featured" section of a card, or the glow effect on a focused element.

### Vivid Accents (States & Special Syntax)

<p>
  <img src="https://placehold.co/100x100/ff70a6/484f5c/png?font=source-sans-pro&text=%23ff70a6" />
  <img src="https://placehold.co/100x100/ffd670/484f5c/png?font=source-sans-pro&text=%23ffd670" />
  <img src="https://placehold.co/100x100/84dcc6/484f5c/png?font=source-sans-pro&text=%2384dcc6" />
  <img src="https://placehold.co/100x100/68b6ef/484f5c/png?font=source-sans-pro&text=%2368b6ef" />
  <img src="https://placehold.co/100x100/00a8e0/484f5c/png?font=source-sans-pro&text=%2300a8e0" />
</p>

A palette of expressive colors used to communicate important states and draw attention to critical information. They should be used purposefully to ensure their impact is not diluted.

- **Flatcap 15**: `#ff70a6` - **Errors & Deletion**: Use for form validation errors, failed connection messages, or the background of a "Delete" confirmation button. It immediately signals a problem or a destructive action.
- **Flatcap 16**: `#ffd670` - **Warnings & Attention**: Ideal for warning notifications, highlighting potentially risky actions, or indicating that a feature is in "beta." It urges caution without being as alarming as the error color.
- **Flatcap 17**: `#84dcc6` - **Success & Confirmation**: Perfect for success messages ("Your changes have been saved"), validation checkmarks, or confirming a successful transaction. It provides positive reinforcement to the user.
- **Flatcap 18**: `#68b6ef` - **Informational Tips & New Features**: A friendly, neutral color for informational alerts, "did you know?" tips, or highlighting a new feature. It invites discovery without interrupting the user's workflow.
- **Flatcap 19**: `#00a8e0` - **Key Syntax & Call-to-Action**: A vibrant cyan that serves as a powerful accent. Use it to highlight the most important keywords in code, or for a special call-to-action button that needs to stand out from the primary blue actions.

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/cheycron)
