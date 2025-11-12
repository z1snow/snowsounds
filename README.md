# Rick Snow - Personal Website

## Your First Website Deployment Guide

This is your starter splash page for **snowsounds.net**

### Files Included:
- `index.html` - Your main webpage
- `style.css` - Styling and design
- `CNAME` - Custom domain configuration
- `README.md` - This file!

---

## Deployment Steps

### Step 1: Upload Files to GitHub

1. Go to your repository on GitHub
2. Click "Add file" → "Upload files"
3. Drag and drop ALL THREE files (index.html, style.css, CNAME)
4. Add a commit message like "Initial splash page"
5. Click "Commit changes"

### Step 2: Enable GitHub Pages

1. In your repository, click "Settings" (top right)
2. Scroll down to "Pages" in the left sidebar
3. Under "Source", select "Deploy from a branch"
4. Choose "main" branch and "/ (root)" folder
5. Click "Save"
6. Wait 1-2 minutes for deployment

Your site will be live at: `https://yourusername.github.io/snowsounds/`

### Step 3: Connect Your Custom Domain (Namecheap)

1. **In Namecheap:**
   - Log into your Namecheap account
   - Go to Domain List → Manage → Advanced DNS
   - Add these records:

   **A Records (add all four):**
   ```
   Type: A Record
   Host: @
   Value: 185.199.108.153
   
   Type: A Record
   Host: @
   Value: 185.199.109.153
   
   Type: A Record
   Host: @
   Value: 185.199.110.153
   
   Type: A Record
   Host: @
   Value: 185.199.111.153
   ```

   **CNAME Record:**
   ```
   Type: CNAME Record
   Host: www
   Value: yourusername.github.io.
   ```
   *(Replace "yourusername" with your actual GitHub username)*

2. **In GitHub:**
   - Go back to Settings → Pages
   - Under "Custom domain", enter: `snowsounds.net`
   - Check "Enforce HTTPS" (may need to wait for DNS to propagate)

3. **Wait for DNS propagation** (15 minutes - 48 hours, usually under 1 hour)

---

## Customization Guide

### Update Your Information:

**In `index.html`:**
- Line 18: Your name (if you want to change it)
- Line 19: Your subtitle/tagline
- Lines 24-28: Your bio text
- Line 34: Your email address
- Lines 43-47: Your social/professional links (GitHub, SoundCloud, etc.)

**In `style.css`:**
- Line 17: Background colors (try different color codes)
- Line 70: Heading size
- You can experiment with any values!

### Color Schemes:
Want a different look? Change these lines in `style.css`:

**Current (dark blue):**
```css
background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
```

**Dark purple:**
```css
background: linear-gradient(135deg, #2d1b69 0%, #1a0b3d 100%);
```

**Dark green:**
```css
background: linear-gradient(135deg, #1a3a2e 0%, #0f2616 100%);
```

**Black:**
```css
background: linear-gradient(135deg, #000000 0%, #1a1a1a 100%);
```

---

## Testing Locally (Optional)

If you want to preview changes before uploading:

1. Download all files to a folder on your computer
2. Double-click `index.html` to open in your browser
3. Make changes and refresh to see updates
4. When happy, upload to GitHub

---

## Next Steps

Once your splash page is live, you can:
1. Add a Projects page
2. Create interactive p5.js widgets
3. Add audio/video galleries
4. Build out your full portfolio

Feel free to experiment! Git version control means you can always go back if something breaks.

---

## Need Help?

If something isn't working:
- Check that all files are in the root of your repository
- Verify your GitHub Pages is enabled
- Give DNS changes time to propagate
- Check Namecheap DNS records match exactly

Ready to build something more complex? Just ask!
