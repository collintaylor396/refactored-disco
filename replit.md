# Dropbox Redirect Page

A minimal HTML redirect page that forwards visitors to a Dropbox URL.

## How it works

`index.html` reads the URL hash (the part after `#`) and redirects the browser to `https://www.dropbox.com` + that hash value. This lets you use a Replit URL as a shareable redirect link to any Dropbox path.

**Example:** visiting `https://<your-replit-url>/#/s/abc123` redirects to `https://www.dropbox.com/s/abc123`.

## Running

The app is served as a static file using Python's built-in HTTP server on port 5000.

```
python3 -m http.server 5000
```

## Files

- `index.html` — the redirect page (the only file)
