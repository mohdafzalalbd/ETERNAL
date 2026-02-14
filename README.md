# 💕 Eternal Love - Wedding Website

A beautiful, responsive wedding website showcasing eternal love with elegant design and multimedia elements.

---

## 📋 Table of Contents

- [About](#about)
- [Features](#features)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Configuration](#configuration)
- [Deployment](#deployment)
- [File Descriptions](#file-descriptions)
- [License](#license)

---

## About

**Eternal Love** is a dedicated wedding website designed to celebrate the union of two people. The site features beautiful imagery, immersive audio, and a clean, romantic interface that captures the essence of eternal commitment.

---

## Features

✨ **Responsive Design** - Works seamlessly on all devices (desktop, tablet, mobile)

🎵 **Audio Integration** - Beautiful love nasheed (Islamic devotional song) background

🖼️ **Image Gallery** - Curated wedding photography showcase

⚙️ **Nginx Setup** - Pre-configured nginx server for optimal performance

🎨 **Elegant UI** - Modern, romantic design aesthetic

---

## Project Structure

```
eternal-love/
│
├── index.html                    # Main website page
├── assets/
│   ├── images/
│   │   ├── wedding1.jpeg        # First wedding photo
│   │   └── wedding2.jpeg        # Second wedding photo
│   │
│   └── audio/
│       └── love_nasheed.mp3      # Background music
│
├── nginx-config/
│   └── eternal-love.conf        # Nginx server configuration
│
└── README.md                     # Documentation (this file)
```

---

## Technologies Used

- **HTML5** - Semantic markup and structure
- **CSS3** - Styling and responsive design
- **JavaScript** - Interactive features (optional)
- **Nginx** - Web server and reverse proxy
- **Multimedia** - JPEG images and MP3 audio

---

## Installation

### Prerequisites

- Nginx web server installed
- Git for version control
- Modern web browser

### Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/eternal-love.git
   cd eternal-love
   ```

2. **Install Nginx (if not already installed):**
   - **Ubuntu/Debian:**
     ```bash
     sudo apt-get update
     sudo apt-get install nginx
     ```
   - **macOS:**
     ```bash
     brew install nginx
     ```
   - **Windows:**
     Download from [nginx official website](http://nginx.org/en/download.html)

3. **Copy project files to web root:**
   ```bash
   sudo cp -r . /var/www/eternal-love/
   ```

---

## Configuration

### Nginx Setup

1. **Copy the configuration file:**
   ```bash
   sudo cp nginx-config/eternal-love.conf /etc/nginx/sites-available/
   ```

2. **Enable the site:**
   ```bash
   sudo ln -s /etc/nginx/sites-available/eternal-love.conf /etc/nginx/sites-enabled/
   ```

3. **Test nginx configuration:**
   ```bash
   sudo nginx -t
   ```

4. **Restart nginx:**
   ```bash
   sudo systemctl restart nginx
   ```

### Custom Configuration

Edit `nginx-config/eternal-love.conf` to customize:
- Server port (default: 80)
- Server name/domain
- SSL certificates (for HTTPS)
- Cache settings
- Compression options

---

## Deployment

### Local Testing

1. Start your local Nginx server
2. Navigate to `http://localhost` in your browser
3. Verify all assets load correctly

### Production Deployment

1. **Choose a hosting provider** (AWS, DigitalOcean, Heroku, etc.)
2. **Configure domain** - Point your domain to the server
3. **Set up SSL certificate** - Use Let's Encrypt for free HTTPS
4. **Deploy files** - Use Git or SCP to transfer files
5. **Restart services** - Restart Nginx to apply changes

#### Example with Let's Encrypt (Ubuntu):

```bash
sudo apt-get install certbot python3-certbot-nginx
sudo certbot --nginx -d yourdomain.com
```

---

## File Descriptions

| File | Purpose |
|------|---------|
| `index.html` | Main website page with HTML structure and content |
| `wedding1.jpeg` | Featured wedding photograph #1 |
| `wedding2.jpeg` | Featured wedding photograph #2 |
| `love_nasheed.mp3` | Background music - Islamic devotional song |
| `eternal-love.conf` | Nginx web server configuration file |
| `README.md` | Project documentation |

---

## Browser Compatibility

- ✅ Chrome/Chromium (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

---

## Performance Optimization

The nginx configuration includes:
- Gzip compression for faster load times
- Browser caching policies
- Proper MIME type handling
- Optimized file serving

---

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit changes (`git commit -m 'Add improvement'`)
4. Push to branch (`git push origin feature/improvement`)
5. Open a Pull Request

---

## Support

For issues, questions, or suggestions:
- Open an issue on GitHub
- Contact the development team
- Check existing issues for solutions

---

## License

This project is licensed under the MIT License - see LICENSE file for details.

---

## 💫 Acknowledgments

- Built with love ❤️
- Inspired by eternal commitment
- Beautiful design for special moments

---

**Last Updated:** February 2026

**Version:** 1.0.0
