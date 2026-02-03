# Link to MP4

A clean, minimal web app for downloading videos from YouTube, Twitter, Instagram, TikTok, and more.

## Live Demo

Visit the deployed app at: `https://yourusername.github.io/link-to-mp4`

## Features

- Download videos from popular platforms
- Quality selection (Best, 720p, 480p)
- Clean, Apple-inspired interface
- No signup or API keys required
- Mobile-friendly responsive design

## Supported Platforms

- YouTube (videos, shorts, music)
- Twitter/X
- Instagram
- TikTok
- Reddit
- Vimeo
- SoundCloud
- And many more

## Quick Deploy to GitHub Pages

1. Fork or clone this repository
2. Go to Settings → Pages
3. Under "Source", select "Deploy from a branch"
4. Choose `main` branch and `/ (root)` folder
5. Click Save
6. Your app will be live at `https://yourusername.github.io/link-to-mp4`

## Manual Deployment

```bash
# Clone the repository
git clone https://github.com/yourusername/link-to-mp4.git
cd link-to-mp4

# The app is ready to deploy - just push to GitHub
git add .
git commit -m "Initial deployment"
git push origin main
```

## How It Works

This app uses the [cobalt.tools](https://cobalt.tools) API to process video downloads. All video extraction happens server-side through their free API.

## Local Development

Simply open `index.html` in your browser. No build process required.

## Technical Stack

- Pure HTML/CSS/JavaScript
- No dependencies or frameworks
- Client-side only (except API calls)
- Responsive design with Apple-inspired UI

## Privacy

- No data is stored by this application
- Video URLs are processed through cobalt.tools API
- Downloads are saved directly to your device

## License

MIT License - Feel free to use and modify

## Credits

- Video processing powered by [cobalt.tools](https://cobalt.tools)
- Design inspired by Apple's design language
