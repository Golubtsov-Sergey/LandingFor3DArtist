# Landing Page for 3D Artist Portfolio

A minimalist, high-end editorial portfolio landing page built using Tailwind CSS, Playfair Display, and Inter fonts. It is fully responsive, including a dedicated full-screen overlay menu for mobile, and features an interactive HTML5 video player.

## Features

- **Monochromatic Editorial Design:** Built strictly around neutral, monochromatic colors as defined in the styling system, keeping the UI minimal to frame the visualizations.
- **Interactive Video Player:** The "Chair Animation Study" case study has an interactive video container. Clicking the thumbnail transitions into a native, high-quality HTML5 video player playing a sample render loop.
- **Mobile Menu Overlay:** A mobile navigation menu built with fluid slide-in transitions.
- **0px Corner Radius:** Enforces sharp corners to maintain the architectural feel of structural integrity and technical drawing precision.
- **GitHub Actions Auto-deployment:** Configured to deploy automatically to GitHub Pages on pushes to the `main` branch.

## How to Customize

### 1. Changing the Video
The video file is loaded inside the case study section. 
Open `index.html` and search for:
```html
<!-- Interactive Video Player -->
<div id="video-container" ...>
    <video id="case-study-video" ...>
        <source src="https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ForBiggerEscapes.mp4" type="video/mp4"/>
        Your browser does not support the video tag.
    </video>
...
```
Replace the URL in the `<source src="..." />` tag with your own hosted video URL or path to a local video file (e.g. `assets/reel.mp4`).

### 2. Changing Images
All image URLs are currently pointing to the sample rendering images from Google Usercontent. To replace them, simply search for `<img alt="..." src="..." />` tags and substitute your own file paths or image URLs.

---

## Hosting on GitHub Pages

This repository is pre-configured with a GitHub Actions workflow to deploy the website automatically.

### Steps to Enable:

1. Push your changes to your remote GitHub repository (`https://github.com/Golubtsov-Sergey/LandingFor3DArtist.git`).
2. Open your repository on GitHub.
3. Navigate to **Settings** -> **Pages** (under the "Code and automation" section).
4. Under **Build and deployment**:
   - Change **Source** to: `GitHub Actions`.
5. The next time you push code to the `main` branch, the deployment workflow will run automatically, and your site will be live at `https://golubtsov-sergey.github.io/LandingFor3DArtist/` within a couple of minutes!
