---
title: "Release Notes"
author: "Ana Claudia"
date: 2025-12-01
wordCount: false
---

# Release Notes

All notable changes to this documentation project are documented below.

## [1.1.0] - 2025-12-28
### ✨ Added & Improved
- **Branding**: Renamed the project to **Doc-as-Code** for a professional market positioning.
- **Localization**: Switched menu and navigation to English.
- **Structure**: Reorganized files into a numbered sequence (`0-` to `4-`) for better logical flow.
- **Config**: Updated `hugo.toml` with custom menus, author profiles, and social links.

### 🔧 Fixed
- **Environment**: Fixed "Unable to locate config file" by aligning terminal directory with project root.
- **Path Fix**: Resolved Hugo command execution issues by correctly configuring Windows Environment Variables.
- **Bug**: Fixed "Anonymous" author display by mapping `params.author` in the configuration.

---

## [1.0.0] - 2025-12-23
### 🚀 Initial Setup
- Initial project structure using Hugo and FixIt theme.
- GitHub Actions workflow for automated deployment.