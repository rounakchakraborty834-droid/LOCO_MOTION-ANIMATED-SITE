# LOCO MOTION — Scroll-Driven Animated Website

<p align="center">
  <a href="https://rounakchakraborty834-droid.github.io/LOCO_MOTION-ANIMATED-SITE/">
    <strong>🌐 VIEW LIVE WEBSITE</strong>
  </a>
</p>

<p align="center">
  An immersive web development experience exploring animation, smooth scrolling, kinetic typography, and interactive visual storytelling.
</p>

---

## 🎬 About the Project

**LOCO MOTION** is an experimental, animation-focused website built around the idea:

> Good design is obvious. Great design is transparent.

The project transforms a web development landing page into an interactive visual experience using scroll-controlled image sequences, oversized animated typography, smooth scrolling, pinned content sections, and custom interactions.

Instead of presenting information through a conventional static layout, the website uses motion and scroll progression to guide visitors through its content.

**Created by:** Rounak Chakraborty  
**Project type:** Creative frontend development / animated website  
**Status:** Published  
**Hosting:** GitHub Pages

## 🌐 Live Demo

**Website:**  
https://rounakchakraborty834-droid.github.io/LOCO_MOTION-ANIMATED-SITE/

**Source code:**  
https://github.com/rounakchakraborty834-droid/LOCO_MOTION-ANIMATED-SITE

## ✨ Features

### 🎞️ Scroll-Controlled Canvas Animation

The opening section uses an HTML canvas to display a sequence of **300 numbered PNG frames**.

As visitors scroll, GSAP updates the animation frame, creating a continuous visual sequence synchronized with the page's movement.

### 🌀 Smooth Scrolling

Locomotive Scroll provides the smooth-scrolling experience. Its scroll events are synchronized with GSAP ScrollTrigger to coordinate animations and pinned sections.

### 🔤 Kinetic Typography

Large, repeated headlines create a marquee-style visual treatment, emphasizing the statement:

**GOOD DESIGN IS OBVIOUS. GREAT DESIGN IS TRANSPARENT.**

Typography is a central part of the experience rather than simply a way to display headings.

### 📌 Scroll-Triggered Sections

GSAP ScrollTrigger coordinates the animation timeline and pins selected sections while visitors move through the page.

This creates a staged storytelling experience, allowing the content and visual sequence to progress with scrolling.

### 🎨 Creative Visual Design

The website features:
- Large typography and bold text treatments.
- Full-screen content sections.
- Canvas-based imagery.
- Layered visual elements and section transitions.
- Minimal navigation and a custom footer.
- Motion-led presentation focused on visual storytelling.

### 🖱️ Interactive Elements

- Footer navigation with ripple feedback.
- A footer that appears when visitors approach the bottom of the page.
- A scroll-to-top control.
- Smooth transitions and hover effects.
- Canvas resizing when the browser viewport changes.

## 🧰 Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Website structure and content |
| CSS3 | Layout, typography, styling, and transitions |
| JavaScript | Animation logic and interactive behaviour |
| HTML Canvas API | Rendering the animated image sequence |
| GSAP 3.11.5 | Animation timelines and tweening |
| GSAP ScrollTrigger | Scroll-based animation and pinned sections |
| Locomotive Scroll 3.5.4 | Smooth scrolling |
| GitHub Pages | Static hosting and deployment |

The project uses vanilla HTML, CSS, and JavaScript, with animation libraries loaded from public CDNs. A package manager or framework build step is not required for the current implementation.

## 🧭 Website Sections

### 01 — Introduction

Introduces the project's design philosophy through oversized, repeated headlines, supporting text, and a scroll-controlled canvas animation.

### 02 — Key Words

Presents ideas such as having fun, coding together, telling stories, taking chances, and building collaboratively.

### 03 — Have Fun Together

Explores cooperation, sharing, and creativity through a full-screen section with scroll-based presentation.

### 04 — Web Development Playground

Concludes the main visual sequence with the idea of web development as a creative playground.

### 05 — Interactive Footer

Provides internal navigation, visual feedback on footer links, and a scroll-to-top interaction.

## 📂 Project Structure

\`\`\`text
LOCO_MOTION-ANIMATED-SITE/
│
├── .github/
│   └── workflows/          # GitHub workflow configuration
│
├── index.html               # Main HTML document
├── style.css                # Website styling and layout
├── script.js                # Canvas animation and scroll logic
│
├── male0001.png              # Animation sequence frames
├── male0002.png
├── male0003.png
├── ...
├── male0300.png              # Final numbered frame
│
├── aaaaaaaaaaaa.png          # Additional image asset
└── cursor.png                # Cursor-related image asset
\`\`\`

**Important:** The animation depends on the numbered PNG files being available at the paths referenced in `script.js`. Keep the file naming pattern and directory structure intact when modifying or replacing the image sequence.

## 🚀 Run Locally

You can run the website locally without installing npm dependencies.

### Option 1: Visual Studio Code

1. Clone or download the repository.
2. Open the project folder in Visual Studio Code.
3. Install the Live Server extension if it is not already installed.
4. Open `index.html` using Live Server.
5. Visit the local address displayed by the extension.

### Option 2: Python HTTP Server

Make sure Python is installed, then open a terminal in the project root.

Run:

\`\`\`bash
python -m http.server 8000
\`\`\`

On Windows, you can also use:

\`\`\`powershell
py -m http.server 8000
\`\`\`

Open the website at:

**http://localhost:8000**

A local HTTP server helps ensure the browser can load the relative image paths consistently.

## ⚙️ How the Animation Works

The main visual sequence follows this process:

1. JavaScript creates image objects for the 300 numbered PNG frames.
2. An HTML canvas renders the currently selected frame.
3. GSAP animates a frame counter from the beginning of the sequence toward its end.
4. ScrollTrigger synchronizes the frame counter with scroll progress.
5. Locomotive Scroll supplies the smooth-scrolling behaviour and communicates scroll updates to ScrollTrigger.
6. Selected content sections are pinned during their configured scroll ranges.

The result is a scroll-driven animation that connects the visual sequence to the visitor's movement through the page.

## ☁️ Deployment

The website is published through **GitHub Pages**.

Live URL:

https://rounakchakraborty834-droid.github.io/LOCO_MOTION-ANIMATED-SITE/

To deploy your own copy:

1. Push the project files to a GitHub repository.
2. Open the repository's **Settings → Pages**.
3. Configure GitHub Pages to publish from the branch and directory containing `index.html`.
4. Allow the deployment to complete.
5. Open the generated Pages URL and test the website.

Ensure all image frames, stylesheets, JavaScript files, and library references remain accessible after deployment.

## 🔧 Customization

**Content:** Edit the headings and paragraphs in `index.html`.

**Visual design:** Modify colours, layout, typography, spacing, and visual treatments in `style.css`.

**Animation behaviour:** Update the frame counter, canvas rendering, GSAP tweens, and ScrollTrigger configuration in `script.js`.

**Image sequence:** Replace the numbered PNG files while preserving their filenames and expected paths, or update the frame-loading logic to match a new sequence.

**Navigation and social links:** Update the footer links in `index.html`. The social links currently use placeholder destinations and should be replaced with the intended profile URLs.

## ⚡ Performance Considerations

The website loads a sequence of 300 images. Animation smoothness and loading time may vary depending on the visitor's device, memory, network connection, and browser.

Potential areas for future optimization include:
- Preloading frames strategically.
- Loading frames progressively where practical.
- Reducing image file sizes.
- Testing animation performance on mobile devices.
- Refining touch and reduced-motion behaviour.

## 🔮 Future Improvements

- Improve image-sequence loading and memory efficiency.
- Refine small-screen layouts and touch interactions.
- Add more deliberate loading and error-handling states.
- Review accessibility and reduced-motion support.
- Replace placeholder social links with real destinations.
- Further optimize rendering performance across devices.

## 👨‍💻 Author

**Rounak Chakraborty**

- **GitHub:** https://github.com/rounakchakraborty834-droid
- **Live Project:** https://rounakchakraborty834-droid.github.io/LOCO_MOTION-ANIMATED-SITE/
- **Repository:** https://github.com/rounakchakraborty834-droid/LOCO_MOTION-ANIMATED-SITE

---

<p align="center">
  Made with code, motion, and a passion for creative web experiences.
</p>
