# Custom URL Shortener

## Overview

This is a custom URL shortener built on Express.js, Node.js, and MongoDB. It provides a simple and efficient way to create shortened URLs, along with features for URL retrieval and analytics tracking.

## Features

- **Shorten URLs:** Post your URL via `/url` endpoint to receive a shortened version.
  
- **Retrieve Shortened URL:** Access your shortened URL by making a GET request to `/url/:id`.

- **Analytics:** Track analytics for a shortened URL by accessing `url/analytics/:id`. Receive information on visit clicks and visit history.

## Usage

### Post a URL

```bash
curl -X POST -H "Content-Type: application/json" -d '{"originalUrl": "YOUR_URL_HERE"}' http://localhost:8002/url
