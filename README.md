# Winter Lab Website

This repository contains the source code for the Winter Lab website at the University of Georgia (College of Public Health, Department of Epidemiology and Biostatistics). 

The site is built using [Quarto](https://quarto.org/), utilizing custom CSS for theming, dynamic filtering for the team directory, and automated listing engines for news, publications, and presentations.

## Directory Structure

```text
/
├── _quarto.yml             # Global site configuration and navigation menu
├── styles.css              # Custom styling, dark mode, and UGA branding
├── index.qmd               # Homepage with animated hero banner
├── .gitignore              # Prevents cache and environment files from syncing
│
├── Page Layouts/
│   ├── people.qmd          # Main team directory with JS filtering
│   ├── news.qmd            # Aggregated news and updates feed
│   ├── publications.qmd    # Peer-reviewed publication feed
│   ├── presentations.qmd   # Slide decks and posters feed
│   ├── lab-calendar.qmd    # Embedded lab schedule
│   └── lab-materials.qmd   # Internal resources and protocols
│
├── Content Directories/    # Drop new .qmd files here to auto-update the site
│   ├── news/               # Lab announcements and milestones
│   ├── publications/       # Manuscripts and abstracts
│   ├── presentations/      # Conference materials
│   └── team/               # Individual member profiles (auto-pulls tagged content)
│       ├── amy_winter.qmd
│       └── ...
│
└── assets/                 # Static files (Profile pictures, PDFs, graphics)