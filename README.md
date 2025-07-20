# Train With Mahmoud Landing Page

A bilingual (English/Arabic), dark‑mode‑friendly static landing page for a personal training service, featuring:

- **Hero section** with customizable background image and overlay text  
- **Plans** and **Features** sections  
- **Email subscription** form  
- **Tailored YouTube demo** embed (with `<iframe id="video" src="...">`)  
- **Language toggle** (English/Arabic) with persistent selection  
- **Dark/light theme toggle** with persistent preference  
- **Responsive layout** and smooth animations  

---

## 🚀 Getting Started

1. **Download or clone** this repository:  
   ```bash
   git clone https://github.com/yourusername/train-with-mahmoud.git
   cd train-with-mahmoud
   ```

2. **Open** the `index.html` file in your browser. No build tools or server required (plain HTML/CSS/JS).

3. **Customize** the content:  
   - **Hero background**: Replace `path/to/hero-bg.jpg` in `styles.css` with your image path or URL.  
   - **YouTube demo**: Update the `src` of `<iframe id="video">` in `index.html` with your own YouTube embed URL.  
   - **Texts**: Edit headings, paragraphs, and plan/feature cards in the HTML (inside `<main>`).  
   - **Logo**: Swap out the `<img>` at the top (`MWFit` placeholder) with your own logo.

4. **Optional**: Serve via local HTTP to avoid any `file://` quirks:  
   ```bash
   # Python 3.x
   python3 -m http.server 8000
   # Then visit http://localhost:8000 in your browser.
   ```

---

## ⚙️ Features

- **Bilingual Support**: English and Arabic content, toggled with persistent choice stored in `localStorage`.  
- **Dark/Light Mode**: Switch themes, preference saved in `localStorage`.  
- **Responsive Design**: Adapts to mobile via Flexbox and media queries.  
- **Smooth Animations**: Fade‐in, slide‐in, and slide‐up on scroll using CSS `@keyframes`.  
- **Embedded Video**: Uses a responsive `<iframe>` with `id="video"`.

---

## 📂 Project Structure

```
├── index.html      # Main landing page
├── styles.css      # Base styles and layout
├── README.md       # You are here
└── assets/
    ├── hero-bg.jpg  # Your hero background image
    └── logo.png     # Your logo (optional)
```

---

## 🛠️ Customization Tips

- **Background Positioning**: In `styles.css`, adjust:
  ```css
  #hero {
    background-position: 50% 30%; /* tweak horizontal/vertical offsets */
    background-size: cover;       /* or contain */
    min-height: 60vh;             /* adjust section height */
  }
  ```

- **Animation Durations**: Modify `animation: fadeIn 1.5s ease-in` or other keyframes in `styles.css`.  
- **Adding Sections**: Follow the existing `<section class="section slide-up">` pattern to insert new content blocks.

---

## 🤝 Contributing

1. Fork this repo  
2. Create your feature branch (`git checkout -b feature/YourFeature`)  
3. Commit your changes (`git commit -m "Add awesome feature"`)  
4. Push to the branch (`git push origin feature/YourFeature`)  
5. Open a Pull Request  

---

## 📄 License

This project is open‑source and available under the MIT License. Feel free to use, modify, and distribute as you like.
