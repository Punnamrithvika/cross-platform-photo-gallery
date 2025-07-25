# Cross-Platform Photo Gallery

A modern, feature-rich photo gallery application that works seamlessly across multiple platforms through a responsive web interface.

## Features

- **Cross-Platform Compatibility**: Access through any modern web browser on desktop or mobile devices
- **Responsive Design**: Optimized viewing experience across all device sizes
- **Intelligent Organization**: Auto-categorization and smart albums using metadata
- **Advanced Search**: Find photos by date, location, people, objects, and more
- **Privacy-Focused**: Your photos remain yours with configurable sharing settings
- **Customizable UI**: Personalize your viewing experience with themes and layouts
- **Performance Optimized**: Fast loading with efficient image compression and caching

## Tech Stack

- **Backend**: PHP
- **Database**: MySQL/MariaDB for storing metadata and user information
- **Frontend**: HTML5, CSS3, JavaScript
- **Image Processing**: PHP GD/Imagick for server-side processing
- **Authentication**: Custom PHP authentication system

## Installation

### Prerequisites

- PHP 7.4+ or 8.0+
- Web server (Apache, Nginx, etc.)
- MySQL/MariaDB
- PHP extensions: GD or ImageMagick, mbstring, xml

### Setup Instructions

1. **Clone the repository**

```bash
git clone https://github.com/Punnamrithvika/cross-platform-photo-gallery.git
```

2. **Set up your web server**

Configure your web server to point to the project directory. Example for Apache:

```apache
<VirtualHost *:80>
    ServerName gallery.local
    DocumentRoot /path/to/cross-platform-photo-gallery
    
    <Directory /path/to/cross-platform-photo-gallery>
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>
```

3. **Configure database**

Import the database schema:

```bash
mysql -u username -p database_name < database/schema.sql
```

4. **Configure application settings**

```bash
cp config/config.example.php config/config.php
# Edit config.php with your settings
```

5. **Set proper permissions**

```bash
chmod 755 -R ./
chmod 777 -R ./uploads
chmod 777 -R ./cache
```

## Usage Guide

1. **Create an account or log in** using email credentials
2. **Upload photos** via the web interface
3. **Organize your collection** with albums, tags, and favorites
4. **View and share** your photos with built-in tools
5. **Manage privacy settings** for individual photos or albums

## API Documentation

API documentation is available in the [API Documentation](docs/API.md) file.

## Architecture

<div align="center">
  <img src="docs/assets/architecture-diagram.png" alt="Architecture Diagram" width="800"/>
  <p><em>System Architecture Diagram</em></p>
</div>

The application follows a modular architecture with:
- Authentication system
- Image processing module
- Gallery management
- User management
- Search functionality

## Contributing

We welcome contributions to improve the Cross-Platform Photo Gallery!

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<div align="center">
  <p>Made with ❤️ for photographers and photo enthusiasts everywhere</p>
</div>
