# modstore
A webapp to discover, rate and publish mods for Citybound

# Initial design

**Please discuss in the [modstore room on Gitter](https://gitter.im/citybound/modstore)**

## Pages

### Start page

- most popular mods
- best rated mods
- recently updated mods
- completely new mods

### Mod page

- mod metadata (see below)
- download
- screenshots
- ratings

### Search page

- fulltext search
- by tag
- sort by: rating, downloads, last updated

## Data Objects / Sources

### A Mod

In manifest file
- Name
- Version
- Game Version Compatability
- (Dependencies)

In README.md
- Description
- Tags (standardized format?)
- + for example
  - Link to issue tracking if any

In CHANGELOG.md
- Changelog

In a special folder
- Screenshots

In modstore database
- Number of downloads
- Ratings (see below)

From cross-compilation service
- Cross-platform downloadables

### A Rating

In modstore database

- Star Rating? Or just thumbs up/down?
- Rating date
- Rated version of the mod (user has to know?)
- Rating text
- Submitter name (optional)
- Rating Screenshots?
