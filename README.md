# </> DevDock

A modern developer toolbox built with HTML, CSS, and JavaScript. Format JSON, generate random passwords, and save coding notes—all in one browser-based workspace.

## ✨ Features

### JSON Studio
- Format JSON with readable indentation.
- Minify JSON into a compact string.
- Validate input and display parsing errors.
- Load sample data and copy the result.

### Password Lab
- Generate passwords from 8 to 64 characters.
- Choose uppercase letters, lowercase letters, numbers, and symbols.
- Include at least one character from every selected category.
- Use the browser’s cryptographic random number generator.
- Copy generated passwords without saving them.

### Dev Notes
- Write and automatically save plain-text notes.
- Restore notes when you return using the same browser.
- View the character count.
- Download notes as a `.txt` file.

### Design
- Dark theme with lavender accents.
- Responsive layout for mobile and desktop.
- Keyboard focus indicators and labeled controls.
- No external dependencies or API keys.

## 🚀 Getting Started

1. Download or clone this repository.
2. Open `index.html` in your browser.

No installation or build step is required.

### Optional Local Server

With Python 3 installed, run this command from the project folder:

```bash
python3 -m http.server 8000
```

Then open **http://localhost:8000**.

## 🛠️ Technologies

- HTML5
- CSS3
- Vanilla JavaScript
- Web Crypto API
- Clipboard API
- localStorage

## 📁 Project Structure

```text
devdock/
├── index.html
└── README.md
```

All CSS and JavaScript are included in `index.html`.

## 🎯 Usage

1. Select a tool using the navigation buttons.
2. Paste JSON, configure a password, or write a note.
3. Use the available buttons to format, generate, copy, or download.

If automatic copying is unavailable, the app selects the text so you can copy it manually.

## 💾 Privacy and Storage

- Input is processed locally without being sent to a server.
- Only coding notes are saved in localStorage.
- JSON input and generated passwords are not saved by the app.
- Notes do not sync across devices.
- Clearing browser data removes saved notes.
- Download important notes to keep a separate copy.

Avoid storing passwords, API keys, or other secrets in Dev Notes.

## ⚠️ Limitations

- JSON processing uses JavaScript numbers. Integers larger than
  `9,007,199,254,740,991` may lose precision.
- Formatting removes duplicate JSON object keys, keeping the last value.
- Clipboard access depends on browser permissions and context.
- Browser storage availability varies, especially when opening local files.
- Notes support up to 100,000 characters.

## 🎨 Customization

Edit the CSS variables in `:root` to change the theme:

```css
--bg: #10111c;
--panel: #191b2c;
--text: #eeeefa;
--accent: #b2a0ff;
```

You can also update the HTML text or extend the JavaScript with additional developer tools.
