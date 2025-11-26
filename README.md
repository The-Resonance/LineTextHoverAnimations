# GRANTBOT WISHES - AI Automation Dreams

Share your AI automation wishes and see what others dream of automating in their business and personal workflows. Built with beautiful terminal-like hover animations and an interactive wish submission system.

## 👀 What You'll See

When you run this project, you'll get a beautiful cyberpunk-style website with:
- **Animated background video** with terminal aesthetics
- **Hover effects** on text that create cool line animations
- **Auto-typing animation** in the wish submission form
- **Interactive wish list** where you can click items to see details
- **Like buttons** to vote on automation ideas
- **Real-time form submission** that adds wishes to the list

Perfect for learning modern web animations and interactive UI design!

![GRANTBOT WISHES Screenshot](https://grantbot-wishes-alpha.vercel.app/img/preview.png)

## ✨ Features

- **Interactive Wish Submission**: Submit your AI automation dreams with an animated typing effect
- **Smart Categorization**: Automatic category detection based on wish content
- **Terminal Aesthetics**: Beautiful hover animations with a cyberpunk terminal feel
- **Live Updates**: See wishes appear in real-time with smooth animations
- **Load More**: Progressive loading of automation wishes
- **Like System**: Thumbs up your favorite automation ideas

## 🚀 Quick Start

### Prerequisites
- **Node.js** (version 14 or higher) - [Download here](https://nodejs.org/)
- A web browser (Chrome, Firefox, Safari, etc.)
- A code editor (VS Code, Sublime Text, etc.) - optional but recommended

### Option 1: Using npm (Recommended for beginners)

1. **Open Terminal/Command Prompt**
   - **Mac**: Press `Cmd + Space`, type "Terminal", press Enter
   - **Windows**: Press `Win + R`, type "cmd", press Enter
   - **Linux**: Press `Ctrl + Alt + T`

2. **Navigate to the project folder**
   ```bash
   cd /path/to/LineTextHoverAnimations
   ```

3. **Install dependencies** (first time only)
   ```bash
   npm install
   ```

4. **Start the development server**
   ```bash
   npm run dev
   ```
   
5. **Open your browser**
   - The server will automatically try to open your browser
   - If it doesn't, manually go to the URL shown in terminal (usually `http://localhost:3000` or similar)
   - Look for a message like: `Serving at http://127.0.0.1:65313`

6. **You're done!** 🎉
   - The page will automatically refresh when you make changes
   - Press `Ctrl + C` in terminal to stop the server

### Option 2: Alternative methods

**If npm doesn't work, try Python** (most computers have this):
```bash
cd /path/to/LineTextHoverAnimations
python3 -m http.server 8000
```
Then visit: `http://localhost:8000`

**If you have Python 2**:
```bash
python -m SimpleHTTPServer 8000
```

**Direct file opening** (limited functionality):
- Double-click `index.html` file
- Some features might not work due to browser security restrictions

### Deploy to Vercel

1. **Install Vercel CLI** (if not already installed):
```bash
npm install -g vercel
```

2. **Deploy**:
```bash
# For first deployment
vercel

# For production deployment
npm run deploy
# or
vercel --prod
```

3. **One-click Deploy**: 
   [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/petesena/grantbot-wishes)

## 🛠️ Technology Stack

- **Frontend**: Vanilla HTML, CSS, JavaScript
- **Animations**: GSAP (GreenSock Animation Platform)
- **Text Effects**: SplitType library
- **Deployment**: Vercel (optimized static site)
- **Styling**: Custom CSS with terminal/cyberpunk aesthetics

## 🔧 Troubleshooting

### Common Issues

**"npm: command not found"**
- Install Node.js from [nodejs.org](https://nodejs.org/)
- Restart your terminal after installation

**"Port already in use"**
- The server will automatically find another port
- Look for the new URL in the terminal output
- Or kill the process using that port: `lsof -ti:3000 | xargs kill -9`

**Page doesn't load or looks broken**
- Make sure you're in the correct directory
- Check that all files are present (especially in `css/`, `js/`, `img/` folders)
- Try refreshing the browser (Ctrl+F5 or Cmd+Shift+R)

**Animations not working**
- Check browser console for errors (F12 → Console tab)
- Ensure JavaScript is enabled in your browser
- Try a different browser (Chrome recommended)

**Still having issues?**
- Make sure you have internet connection (for loading fonts)
- Try the Python server method instead
- Check that your browser supports modern JavaScript features

## 📁 Project Structure

```
LineTextHoverAnimations/
├── index.html              # Main application file - START HERE!
├── css/
│   └── base.css            # Core styles and animations
├── js/
│   ├── effect-1/           # Animation effect variant 1
│   ├── effect-2/           # Animation effect variant 2 (currently active)
│   ├── effect-3/           # Animation effect variant 3
│   ├── effect-4/           # Animation effect variant 4
│   ├── gsap.min.js         # GSAP animation library
│   ├── split-type.min.js   # Text splitting library
│   ├── textSplitter.js     # Text manipulation utilities
│   ├── utils.js            # General utilities
│   └── wish-detail.js      # Modal functionality
├── img/
│   ├── grantbotlogo.svg    # GrantBot logo
│   ├── bg.jpg              # Background image
│   └── noise.png           # Texture overlay
├── vid/
│   └── bg-animation.mp4    # Background video animation
├── audio/
│   └── *.mp3               # Background audio files
├── vercel.json             # Vercel deployment config
├── package.json            # Project configuration & scripts
└── README.md               # This file (you are here!)
```

### Key Files Explained
- **`index.html`**: The main page - this is what you see in the browser
- **`css/base.css`**: All the styling and visual effects
- **`js/effect-2/`**: The current animation system being used
- **`package.json`**: Contains the `npm run dev` command and project info

## 🎯 What to Do Next (For Beginners)

### 1. Explore the Code
- Open `index.html` in your code editor to see how it's structured
- Check out `css/base.css` to understand the styling
- Look at `js/effect-2/index.js` to see the animation code

### 2. Make Simple Changes
- **Change colors**: Edit the CSS color values in `base.css`
- **Add your own wish**: Use the form on the website to submit a wish
- **Modify typing text**: Change the `automationIdeas` array in `index.html`

### 3. Try Different Effects
The project has 4 different animation effects! To switch between them:
- Open `index.html`
- Find line 295: `<script type="module" src="js/effect-2/index.js"></script>`
- Change `effect-2` to `effect-1`, `effect-3`, or `effect-4`
- Refresh your browser to see the different animation style

### 4. Learn the Technologies
- **HTML**: Structure of the webpage
- **CSS**: Styling and visual effects
- **JavaScript**: Interactive functionality
- **GSAP**: Professional animation library
- **SplitType**: Text animation effects

## 🎨 Easy Customizations

### Change the Typing Animation Text
Edit the `automationIdeas` array in `index.html` (around line 299):

```javascript
const automationIdeas = [
  "I wish I could automate my morning routine...",
  "I wish I could auto-organize my photos...",
  "Your custom text here...",
];
```

### Add New Wish Categories
Edit the `categoryKeywords` object in `index.html` (around line 398):

```javascript
const categoryKeywords = {
  'Your Category': ['keyword1', 'keyword2', 'keyword3'],
  'Gaming': ['game', 'gaming', 'stream', 'twitch'],
  // ... existing categories
};
```

### Change Colors
Edit `css/base.css` and look for color values like:
- `#8adcc0` (main green)
- `#ffffff` (white text)
- `#000000` (black backgrounds)

## 🚀 Deployment Options

### Vercel (Recommended)
- Automatic deployments from Git
- Global CDN
- Zero configuration
- Custom domains

### Other Platforms
- **Netlify**: Drag and drop the project folder
- **GitHub Pages**: Push to a GitHub repository and enable Pages
- **Firebase Hosting**: Use Firebase CLI to deploy

## 📝 License

[MIT](LICENSE) - Feel free to use this project for your own automation wish collection!

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m 'Add amazing feature'`
4. Push to the branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## 🙏 Credits

- **Built with**: ❤️ by the GrantBot team
- **Design**: Terminal aesthetics with cyberpunk influences





