# Time-Based Dynamic Webpage

This project implements a single-page site (`index.html`) that changes its background color based on the **local time of the visitor**.

## Time Windows
- **Morning (06:00–12:00)** → #FFF4CC
- **Afternoon (12:00–18:00)** → #E6F7FF
- **Evening (18:00–21:00)** → #FFE6E6
- **Night (21:00–06:00)** → #0B1021

The logic is implemented in a small script embedded in `index.html`. No external libraries are required.

## Testing Without Waiting
- Use the **Simulate** buttons on the page
- Or add `?hour=19` to the URL to preview the evening theme (0–23)

## Deployment (GitHub Pages)
1. Push this repo to GitHub: `BlueEyedGrunt/Assignment 2: Time of Day`
2. Go to **Settings → Pages**
3. Under "Build and Deployment," select **Deploy from branch**: `main`, folder `/ (root)`
4. Save. After a minute, your site will be live at:  
   `https://BlueEyedGrunt.github.io/Assignment-2-Time-of-Day/`

## Known Issues / Assumptions
- Course name is set to **COP4813**
- Color palette can be adjusted by editing the CSS variables in `<style>`
- Uses the visitor’s device clock (if their clock is wrong, the background may be off)
