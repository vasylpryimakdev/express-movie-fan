# Movie Fan Site

A small Express.js movie browsing website built with EJS templates and The Movie Database (TMDb) API.

## Features

- Home page lists popular movies from TMDb
- Movie detail pages with additional information for each selected film
- Search support for movies and people
- Uses `helmet` for basic security headers
- Static assets served from `public/`

## Project structure

- `app.js` - Express application setup
- `bin/www` - application startup script
- `routes/index.js` - main route handlers
- `views/` - EJS templates for pages
- `public/` - static CSS, images, and client assets
- `package.json` - project metadata and dependencies

## Dependencies

- `express` ~4.16.0
- `ejs` ~2.5.7
- `helmet` ^3.13.0
- `morgan` ~1.9.0
- `cookie-parser` ~1.4.3
- `http-errors` ~1.6.2
- `debug` ~2.6.9
- `request` ^2.88.0

## Installation

1. Install dependencies:

```bash
npm install
```

2. Start the app:

```bash
npm start
```

3. Open your browser:

```text
http://localhost:3005
```

## Configuration

- The app listens on port `3005` by default.
- You can override the port with the `PORT` environment variable:

```bash
PORT=4000 npm start
```

## Notes

- The application currently uses a hard-coded TMDb API key in `routes/index.js`.
- The search form sends requests to `/search` and supports categories such as `movie` and `person`.
- The detail route for an individual movie is `/movie/:id`.

## License

This project is provided as-is for learning and demonstration purposes.
