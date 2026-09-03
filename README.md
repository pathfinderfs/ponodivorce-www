# Better Way Divorce static website

This is a static restoration of `ponodivorce.com` from its downloaded Wayback
Machine snapshot. It contains no WordPress runtime, server-side code, database,
forms, analytics, or first-party network dependencies.

## Directory structure

- `assets/css` contains the site stylesheet.
- `assets/images` contains photographs, badges, and background artwork.
- `assets/audio` contains the two archived audio recordings.
- `assets/documents` contains downloadable PDF resources.
- Each page has its own directory containing an `index.html` file.

## Local preview

Run a static HTTP server from this directory:

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000/>.

## Cloudflare Pages

Use the repository root as the output directory. No framework preset or build
command is required. The `_headers` file provides a restrictive security policy
while allowing the intentional YouTube, Spotify, University of Hawaii, and
Flickr content used by the archived pages.
