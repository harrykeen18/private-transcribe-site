# LocalScribe Landing Page

Landing page for **LocalScribe** - a privacy-first macOS app for meeting transcription and summarization.

## About LocalScribe

LocalScribe is a macOS application that provides completely private, on-device meeting transcription and summarization. It processes everything locally using:
- **Whisper** (bundled) for speech-to-text transcription
- **Apple Intelligence** for meeting summaries

### Key Features
- 🔒 **100% Private** - Zero network requests, all processing happens on-device
- 🚀 **Universal** - Works with any video conferencing app (Zoom, Meet, Teams, etc.)
- 🔐 **Encrypted Storage** - AES-256 encryption for all stored transcripts
- 🤓 **Smart Summaries** - Powered by Apple Intelligence

### Requirements
- macOS 15.0 (Sequoia) or later
- Apple Silicon (M1/M2/M3/M4)
- Apple Intelligence enabled

### Current Status
LocalScribe is currently in **beta**. The app is not yet notarized by Apple, so users need to manually approve it in System Settings → Privacy & Security after first launch.

## Repository Contents

This repository contains a single-page HTML landing page with:
- Feature showcase
- Download button (links to GitHub releases)
- Beta warning modal with installation instructions
- Buy Me a Coffee support link
- Transparency section with links to source code and release verification

## File Structure

```
.
├── index.html     # Landing page (self-contained HTML/CSS/JS)
├── logo.png       # LocalScribe logo
├── favicon.ico    # Site favicon
└── README.md      # This file
```

## Local Development

No build process required - just open `index.html` in a browser to preview changes.

## Deployment

Currently deployed via GitHub Pages. Any commits to the main branch are automatically deployed.

### Updating the Download Link

When releasing a new version, update the download URL in `index.html`:
- Line 334: Main download button
- Line 368: Fallback link in beta modal
- Line 376: JavaScript download URL constant

Example: `LocalScribe-v0.2.2-beta.zip` → `LocalScribe-v0.3.0-beta.zip`

## Related Links

- **Main Repository**: [github.com/harrykeen18/localscribe](https://github.com/harrykeen18/localscribe)
- **Latest Release**: [github.com/harrykeen18/localscribe/releases/latest](https://github.com/harrykeen18/localscribe/releases/latest)
- **Support**: [buymeacoffee.com/harry18](https://buymeacoffee.com/harry18)
