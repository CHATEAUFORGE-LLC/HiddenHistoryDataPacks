# HiddenHistoryDataPacks

This repository contains the data packs for the Hidden History project, structured as a static site for GitHub Pages hosting.

Site URL: https://chateauforge-llc.github.io/HiddenHistoryDataPacks/

## Structure

- `inventory.json` - Main entry point listing all available cities and their data packs
- `{city-name}/` - Individual city directories containing:
  - `base_pack.json` - Content pack with historical sites data
  - `assets/` - Local media assets (images, logos) for that city's sites

## Data Format

Each content pack follows the specified JSON schema with pack metadata, contact information, branding, and an array of historical sites.

### Content Pack Example
```json
{
  "pack_id": "oakland-base",
  "pack_version": "2025.11.04",
  "active": true,
  "contact": {
    "organization": "Oakland Heritage Alliance",
    "email": "info@oaklandheritage.org"
  },
  "brand": {
    "logo": "https://chateauforge-llc.github.io/HiddenHistoryDataPacks/oakland/assets/oakland_logo.png"
  },
  "sites": [...]
}
```

### Site Example
```json
{
  "id": "oak-001",
  "title": "Camron-Stanford House",
  "address": "1418 Lakeside Dr, Oakland, CA 94612",
  "categories": ["Victorian", "Architecture"],
  "era": "1876",
  "active": true,
  "summary": "An example Victorian home on Lake Merritt showcasing 19th-century domestic architecture.",
  "description_md": "# Camron-Stanford House\n\nThe Camron-Stanford House is a beautifully preserved Victorian mansion...",
  "citations": [
    {
      "label": "Oakland Cultural Heritage Survey",
      "url": "https://www.oaklandca.gov/topics/cultural-heritage-survey",
      "publisher": "City of Oakland",
      "license": "CC BY 4.0"
    }
  ],
  "media": [
    { 
      "type": "image", 
      "url": "https://chateauforge-llc.github.io/HiddenHistoryDataPacks/oakland/assets/camron-stanford-house.svg", 
      "license": "CC BY-SA 4.0" 
    }
  ],
  "tags": ["lake", "victorian", "museum", "architecture"]
}
```

## Assets

All media assets are stored locally within each city's `assets/` directory and referenced with full GitHub Pages URLs. Placeholder SVG images are provided with a simple X pattern design as requested.

## Contribution
Contributions to expand the data packs with more cities and historical sites are welcome. Please follow the established structure and ensure all data is accurate and properly cited.

Create an Issue and submit a Pull Request for any additions or modifications.

1. [Create an Issue](https://github.com/CHATEAUFORGE-LLC/HiddenHistoryDataPacks/issues/new/choose) in order to collaborate and ask questions.
2. [Fork the repository and make your changes](https://github.com/CHATEAUFORGE-LLC/HiddenHistoryDataPacks/fork) so you can make changes as needed.
3. [Submit a Pull Request for review](https://github.com/CHATEAUFORGE-LLC/HiddenHistoryDataPacks/pulls) in order for inclusion into HiddenHistoryDataPacks.