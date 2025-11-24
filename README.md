# n20 - URL Shortener

A privacy-focused URL shortener that doesn't collect excessive user data.

## Features

- **URL Shortening**: Create short links with optional custom handles
- **Privacy-First**: Minimal data collection approach
- **Statistics**: View click counts for your shortened links
- **Link Management**: Delete links using secret keys
- **Safe Redirects**: 10-second delay with domain preview before redirect

## Usage

1. Enter a URL in the input field
2. Optionally add a custom handle
3. Click "Shorten it!" to generate a short link
4. Copy the link (automatically copied to clipboard)
5. View statistics or delete the link using the provided secret key

## Technical Details

- **Frontend**: Pure HTML, CSS, and JavaScript
- **API**: Uses `api.n20.me` for backend operations
- **Storage**: Temporary cookies for secret key management
- **Redirects**: Safe preview before redirecting to destination

## File Structure

```
/
├── index.html          # Main application interface
├── script.js           # Client-side functionality
├── styles.css          # Styling and animations
├── files/              # Static assets (icons, images)
├── privacy/            # Privacy policy page
├── tos/                # Terms of service page
└── README.md           # This documentation
```

## API Endpoints

- `POST /shorten.php` - Create new short URLs
- `GET /resolve.php` - Resolve and redirect short URLs
- `POST /delete.php` - Delete short URLs using secret keys

## Privacy

- Minimal data collection
- Secret keys for link management
- No tracking beyond basic click counting
- Clear privacy policy available at `/privacy/`
