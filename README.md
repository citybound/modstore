# modstore
A webapp to discover, rate and publish mods for Citybound

# Initial design

**Please discuss in the [modstore room on Gitter](https://gitter.im/citybound/modstore)**

General idea: mods are GitHub repos, as much data as possible is gotten from there in the background, but displayed in a nice UI.

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

#### Stored on: GitHub Repo for Mod

- Repo Name = Mod Name

In README.md
- Description
- Tags (standardized format?)

In a special folder
- Screenshots

In GitHub Releases
- Downloadable mod-package (contains binaries for all platforms)
- Changelog
- Data in Manifest file (of each version)
  - Version
  - Game Version Compatability
  - (Dependencies)

In GitHub Issues
- Known Bugs

#### Stored on: modstore database
- Number of downloads
- Ratings (see below)

### A Rating
#### Stored on: modstore database
- Star Rating? Or just thumbs up/down?
- Rating date
- Rated version of the mod (user has to know?)
- Rating text
- Submitter name (optional)
- Rating Screenshots?

-> Could ratings maybe even be stored as issues with a special tag in the repo?
