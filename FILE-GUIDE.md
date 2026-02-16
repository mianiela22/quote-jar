# 📁 FILE GUIDE - What Does Each File Do?

## 🎨 EASIEST FILES TO CUSTOMIZE

### `/src/config/categories.js` ⭐ START HERE!
**What it is:** Your task categories (Academic, RA, Creative, etc.)  
**Customize:** Change names, colors, icons, add new categories  
**Example:**
```javascript
{ id: 'fitness', name: 'Fitness', color: '#FF6B9D', icon: '💪' }
```

### `/src/config/colors.js` ⭐ THEME COLORS
**What it is:** All the colors used in the app  
**Customize:** Change the color scheme  
**Example:** Want a dark theme? Change these hex codes!

---

## 📦 COMPONENT FILES (UI Pieces)

### `/src/components/Header.js`
**What it does:** Shows "Mirla's Space" title + completion count  
**Customize:** Change the app name, adjust text size

### `/src/components/ViewToggle.js`
**What it does:** "Today" vs "All Tasks" buttons  
**Customize:** Add a third view? Change button labels?

### `/src/components/CategoryFilter.js`
**What it does:** The colorful category filter buttons  
**Customize:** Button sizes, spacing

### `/src/components/AddTask.js`
**What it does:** Input box + plus button to add tasks  
**Customize:** Placeholder text, button icon

### `/src/components/TaskItem.js`
**What it does:** How each individual task looks  
**Customize:** Task card design, what info shows

### `/src/components/TaskList.js`
**What it does:** Shows the list of tasks (or empty state)  
**Customize:** Empty state message, spacing

### `/src/components/TimeModal.js`
**What it does:** Popup asking "How long did this take?"  
**Customize:** Modal text, button labels

---

## 🛠️ UTILITY FILES (Behind the Scenes)

### `/src/utils/storage.js`
**What it does:** Saves/loads your data  
**Don't edit unless:** You know what you're doing!  
**Note:** Works in both Claude and deployed versions

### `/src/utils/timeEstimation.js`
**What it does:** The "smart learning" brain!  
**How it works:**
- Finds similar completed tasks
- Calculates average time
- Returns estimate
**Customize:** Change how it matches similar tasks

### `/src/utils/dateHelpers.js`
**What it does:** Helper functions for dates  
**Example:** `isToday()` checks if a date is today

---

## 🎨 STYLE FILES

### `/src/styles/App.css`
**What it does:** Global styles + animations  
**Customize:** Background gradient, animation speed

### `/src/styles/buttons.js`
**What it does:** Reusable button styles  
**Customize:** Button sizes, hover effects

---

## 🧠 MAIN APP FILES

### `/src/App.js` ⚠️ THE BRAIN
**What it does:** Coordinates EVERYTHING  
**Contains:**
- All state management
- Add/complete/delete functions
- Data loading/saving
- Task filtering logic
**Edit carefully:** This controls the whole app!

### `/src/index.js`
**What it does:** React entry point  
**Don't edit:** Unless you know React!

---

## 🌐 PUBLIC FILES

### `/public/index.html`
**What it does:** The HTML wrapper  
**Customize:** Page title, meta description

---

## 📦 CONFIG FILES

### `/package.json`
**What it does:** Lists dependencies  
**Edit when:** Adding new packages  
**Important:** Update `homepage` for GitHub Pages

### `/.gitignore`
**What it does:** Tells Git what not to upload  
**Don't edit:** It's fine as-is!

---

## 🎯 QUICK CUSTOMIZATION GUIDE

### Want to change COLORS?
→ Edit `/src/config/colors.js`

### Want to change CATEGORIES?
→ Edit `/src/config/categories.js`

### Want to change APP NAME?
→ Edit `/src/components/Header.js` (line with "Mirla's Space")

### Want to change EMPTY STATE MESSAGE?
→ Edit `/src/components/TaskList.js`

### Want to change TIME TRACKING LOGIC?
→ Edit `/src/utils/timeEstimation.js`

### Want to change BACKGROUND GRADIENT?
→ Edit `/src/styles/App.css` (`.app-container` section)

---

## 🚨 FILES YOU PROBABLY SHOULDN'T EDIT

Unless you're comfortable with React:
- `/src/App.js` (the brain - be careful!)
- `/src/index.js` (entry point)
- `/src/utils/storage.js` (data persistence)

---

## 💡 PRO TIPS

1. **Start small:** Change one color in `colors.js` first
2. **Test often:** Make a change, save, refresh browser
3. **Use comments:** Add `//` notes to remember what you changed
4. **Keep backups:** Copy files before major changes

Need help editing a specific file? Just ask!
