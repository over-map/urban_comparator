# Urban Comparator

Comparative maps of urban expansion displaying synced dual/tri-view interactive MapLibre instances. 

## Features
- Search global locations using Nominatim OpenStreetMap data. 
- Fully synced map panning, zooming, and rotating across 3 viewports.
- Beautiful custom vector map styles showing detailed land usage from Shortbread schema.

## Project Structure
- `index.html`: Main application entry point containing layout and map initialization logic.
- `assets/`: Contains core static styling dependencies (fonts, sprites, and map style JSON). 
- `public/`: Additional unprocessed static files (like favicon).

## Quick Start
You don't need a build step, but running it through a local static server ensures you avoid CORS issues. 

```bash
# Using Node/npm
npm install
npm start
```
The app will be available at `http://localhost:3000`.

## Architecture Note
This project was recently refactored to align with professional web standards:
- **`assets/` vs `public/`**: Assets utilized by the code directly are kept separate from the public directory.
- **kebab-case naming**: Implemented across static file architectures to ensure compatibility and SEO best practices.
- **Config standardization**: Added `.editorconfig` to automatically sync whitespace rules across all collaborators, alongside an OS-level `.gitignore` to keep the repository clean.

## Credits
Mapping components are built with MapLibre GL JS, featuring data from OpenStreetMap and Esri.
Created by Filippo Imberti.
