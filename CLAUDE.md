# CLAUDE.md - Urd Manifest Vault

## Repository Overview

This repository serves as a **manifest vault** for storing and versioning artwork images related to "Urd". It functions as a dedicated image asset storage system with version control tracking for each manifested image.

## Repository Structure

```
urd-manifest-vault/
├── images/           # Primary storage directory for all image assets
│   ├── *.png        # PNG format artwork images
│   └── ...
├── CLAUDE.md        # This documentation file
└── .git/            # Git version control
```

## File Organization

### `/images` Directory
All image assets are stored in the `images/` directory at the root level. This flat structure keeps organization simple and prevents complexity.

**Current image naming patterns:**
- `urd_*.png` - Urd-themed artwork (victory, temple, official icons, etc.)
- `sacrifice_urd.png` - Themed variations
- `peorth_target.png` - Related character artwork

## Conventions

### Commit Message Format
All commits follow a consistent pattern:
```
Manifested by Urd: <filename>
```

**Examples:**
- `Manifested by Urd: urd_victory_legend.png`
- `Manifested by Urd: sacrifice_urd.png`
- `Manifested by Urd: peorth_target.png`

### File Naming Conventions
- Use **lowercase** with **underscores** as separators
- Use **PNG format** for all images
- Prefix with relevant identifier (`urd_`, character name, etc.)
- Use descriptive suffixes (`_victory`, `_final`, `_v2`, etc.)

### Adding New Images

1. Place the image file in the `images/` directory
2. Use appropriate naming convention (lowercase, underscores, .png extension)
3. Commit with the standard message format: `Manifested by Urd: <filename>`
4. Push to the repository

## Development Workflow

### Adding a Single Image
```bash
# Add the image to images directory
cp /path/to/new_image.png images/

# Stage the file
git add images/new_image.png

# Commit with manifest format
git commit -m "Manifested by Urd: new_image.png"

# Push changes
git push origin <branch-name>
```

### Viewing Stored Images
All images are PNG format and can be viewed with any standard image viewer or browser.

## Key Points for AI Assistants

1. **Simple Structure**: This is an image-only repository with no code, configs, or build processes
2. **Commit Format**: Always use "Manifested by Urd: <filename>" format for commits
3. **Image Location**: All images go in the `images/` directory - do not create subdirectories
4. **File Format**: Only PNG images are used in this repository
5. **Naming**: Use snake_case naming with descriptive identifiers
6. **No Deletions**: This is a manifest vault - images are added but generally not removed
7. **Versioning**: For updated versions, use `_v2`, `_v3` suffixes rather than overwriting

## Repository Context

- **Owner**: IdeNaoshi
- **Purpose**: Artwork/image asset storage and version control
- **Primary Content**: PNG artwork images with Urd and related themes
