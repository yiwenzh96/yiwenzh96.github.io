# How to Add Your Photo as Hero Background

Follow these simple steps to use one of your photos as the hero section background:

## Step 1: Choose and Prepare Your Photo

1. Pick a landscape photo you'd like to use (wildlife or landscape photography)
2. Resize it to web-friendly dimensions:
   - Recommended width: **1920px**
   - Keep file size under **500KB** for fast loading
3. Name it `hero-background.jpg`

## Step 2: Add the Photo

Copy your photo to the images folder:
```bash
cp /path/to/your/photo.jpg images/hero-background.jpg
```

Or manually:
- Place `hero-background.jpg` in `/Users/yiwenzhang/yiwenzh96.github.io/images/`

## Step 3: Enable the Background Image

Open `styles.css` and find this line (around line 167):

```css
opacity: 0; /* Set to 0.3-0.5 to show the image */
```

Change it to:
```css
opacity: 0.4; /* Adjust 0.3-0.5 for subtle background */
```

**Opacity Guide:**
- `0.3` = Very subtle, mostly gradient visible
- `0.4` = Balanced blend (recommended)
- `0.5` = More photo visible, less gradient

## Step 4: Save and Push

```bash
cd /Users/yiwenzhang/yiwenzh96.github.io
git add images/hero-background.jpg styles.css
git commit -m "Add custom hero background image"
git push origin main
```

## Tips:

- **Photo choice**: Landscape-oriented photos work best
- **Contrast**: Choose a photo that works well with white text
- **Mood**: Wildlife or landscape photos create a professional, personal touch
- **Testing**: Try different opacity values (0.3-0.5) to find what looks best

Your background will blend beautifully with the gradient overlay!
