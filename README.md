# 🌸 Mirla's Todo App

A personalized todo app that learns from YOUR habits and gets smarter over time!

## ✨ Features

- 📚 6 custom categories (Academic, RA, Creative, Personal, Spiritual, Routine)
- 🧠 Smart time estimates based on your past tasks
- ⚡ Energy level tracking
- ☀️ Today view vs All tasks
- 💾 Persistent data (survives refreshes!)
- 🎨 Beautiful pastel design
- 📱 Mobile-friendly (perfect for iPhone!)

---

## 📁 Project Structure

```
mirla-todo-app/
├── 📖 FILE-GUIDE.md          ← What each file does
├── 🚀 DEPLOYMENT.md          ← How to get it on your phone
├── 📦 package.json           ← Project dependencies
│
├── public/
│   └── index.html            ← HTML wrapper
│
└── src/
    ├── 📱 App.js             ← Main app (the brain!)
    ├── 🎬 index.js           ← Entry point
    │
    ├── config/               ← EASY TO CUSTOMIZE! ⭐
    │   ├── categories.js     ← Your task categories
    │   └── colors.js         ← Color theme
    │
    ├── components/           ← UI pieces
    │   ├── Header.js         ← Title + completion count
    │   ├── ViewToggle.js     ← Today/All switcher
    │   ├── CategoryFilter.js ← Category buttons
    │   ├── AddTask.js        ← Add task input
    │   ├── TaskItem.js       ← Individual task card
    │   ├── TaskList.js       ← List of tasks
    │   └── TimeModal.js      ← Time tracking popup
    │
    ├── utils/                ← Helper functions
    │   ├── storage.js        ← Save/load data
    │   ├── timeEstimation.js ← Smart learning logic
    │   └── dateHelpers.js    ← Date functions
    │
    └── styles/               ← Styling
        ├── App.css           ← Global styles
        └── buttons.js        ← Button styles
```

---

## 🎯 Quick Start

### Want to Customize?
1. **Read `FILE-GUIDE.md`** ← Explains every file
2. **Start with `/src/config/categories.js`** ← Easiest to edit!
3. **Try changing colors in `/src/config/colors.js`**

### Want to Deploy?
1. **Read `DEPLOYMENT.md`** ← Step-by-step instructions
2. **Choose method:**
   - Netlify (easiest - 2 minutes!)
   - GitHub Pages (more control)

---

## 🎨 Easy Customizations

### Change App Name
Edit: `/src/components/Header.js`
```javascript
Mirla's Space → Your Name's Space
```

### Add a Category
Edit: `/src/config/categories.js`
```javascript
{ id: 'fitness', name: 'Fitness', color: '#FF6B9D', icon: '💪' }
```

### Change Colors
Edit: `/src/config/colors.js`
```javascript
gradientStart: '#FFF5F7' → '#your-color'
```

### Change Empty State Message
Edit: `/src/components/TaskList.js`
```javascript
'Nothing on your plate today!' → 'You're all caught up!'
```

---

## 🧠 How the Smart Learning Works

1. **You complete a task** → App asks "How long did it take?"
2. **You add a similar task** → App estimates time based on past data
3. **More data = Better estimates** → Gets smarter over time!

**Example:**
- Complete "MTH 542 homework" → 2 hours
- Complete "MTH 542 problem set" → 1.5 hours  
- Add "MTH 542 assignment" → Estimates ~1.75 hours ✨

---

## 📱 On Your Phone

Once deployed, you can:
- Add to home screen (looks like a real app!)
- Works offline
- Data syncs across devices (if using same browser)
- Fast and responsive

---

## 🛠️ Tech Stack

- **React** - UI framework
- **Lucide Icons** - Beautiful icons
- **Browser Storage** - Data persistence
- **No backend needed!** - Everything runs in your browser

---

## 💾 Data Storage

**In Claude:** Uses `window.storage` API (persists between sessions)  
**When deployed:** Uses `localStorage` (persists until you clear browser data)

**Privacy:** All data stays on YOUR device. Nothing is sent to servers.

---

## 📚 Files to Read

1. **`FILE-GUIDE.md`** - Understanding the code structure
2. **`DEPLOYMENT.md`** - Getting it on your phone
3. **`/src/config/categories.js`** - Your categories (customize!)
4. **`/src/config/colors.js`** - Your color theme (customize!)

---

## 🎓 Learning Resources

Want to understand the code better?

- **React basics:** https://react.dev/learn
- **JavaScript:** https://javascript.info
- **CSS:** https://web.dev/learn/css

---

## ❤️ Made For

This app was custom-built for Mirla with:
- Pastel aesthetic
- Categories matching her life (Academic, RA, Creative, etc.)
- Encouraging tone ("Great job! 🎉")
- Smart features that respect her workflow

---

## 🤝 Need Help?

Stuck on something? Tell me:
- What file you're editing
- What you're trying to do
- What's not working

I'll help you fix it! 💜

---

**Ready to deploy?** → Read `DEPLOYMENT.md`  
**Ready to customize?** → Read `FILE-GUIDE.md`  
**Just want to try it?** → Open `index.html` in a browser!
