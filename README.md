# LabXpert Chat Embed Test

A simple test page for embedding and testing the LabXpert chat widget on external websites.

## Overview

This project provides a standalone HTML page that simulates a client website embedding the LabXpert chat widget. It's designed to help test and validate the embed functionality in a controlled environment.

## Features

- **Embed Script Integration**: Loads the LabXpert embed script from the main application
- **Visual Status Indicators**: Shows real-time feedback on whether the embed loaded successfully
- **Console Logging**: Monitors postMessage communication between the embed and parent page
- **Responsive Design**: Clean, modern interface for easy testing

## Usage

### Local Development

1. Make sure the LabXpert application is running on `http://localhost:3000`
2. Open `index.html` in your browser
3. The chat widget should appear in the bottom-right corner
4. Click the chat button to open the widget

### What Gets Loaded

- **Embed Script**: `http://localhost:3000/api/embed/embed.js`
- **Chat Widget**: `http://localhost:3000/embed/chat` (loaded in an iframe)

## Testing

The page includes:
- Status indicators showing if the embed loaded correctly
- Browser console logging for debugging postMessage events
- Visual feedback for successful/failed widget initialization

## Troubleshooting

If the widget doesn't appear:
1. Check that the LabXpert app is running on port 3000
2. Open browser console (F12) to check for errors
3. Verify CORS settings allow embedding from the test page origin

## Project Structure

```
.
├── index.html          # Test page with embed integration
└── README.md          # This file
```

## Related

This test page is part of the LabXpert ecosystem and requires the main LabXpert application to be running to function properly.
