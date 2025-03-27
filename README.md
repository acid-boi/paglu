# Paglu Tab Manager

## Overview

Paglu is a powerful Bash-based browser tab management tool designed for Brave Browser. It allows you to create, save, and restore browser tab sessions with ease.

## Features

- 🌐 Save and manage browser tab templates
- 🔧 Easy installation and system-wide integration
- 📂 Centralized configuration management
- 🖥️ Desktop application entry
- 🗑️ Simple uninstallation process

## Prerequisites

- Brave Browser
- `jq` JSON processor
- `curl`

## Installation

### Quick Installation

```bash
sudo chmod +x pagluinstaller
sudo ./pagluinstaller install
```

### Customization

During installation, you can:

- Choose a custom installation directory
- Automatically set up system-wide access
- Create desktop application entry

## Usage

```bash
# Create a new tab template
paglu create

# Open a saved template
paglu open <template_name>

# Edit an existing template
paglu edit <template_name>
```

## System Details

- **Default Installation Directory**: `/opt/paglu`
- **Configuration Storage**: `$INSTALL_DIR/.config`
- **Symlink Location**: `/usr/local/bin/paglu`

## Uninstallation

```bash
sudo ./paglu uninstall
```

## Dependencies

Paglu automatically checks for required dependencies:

- jq
- curl
- brave-browser

## Security and Permissions

- Runs with root permissions during installation
- Sets appropriate file and directory permissions
- Uses Access Control Lists (ACL) for flexible access

## Contributing

Contributions are welcome! Please submit issues or pull requests on the project's repository.

## Troubleshooting

- Ensure all dependencies are installed
- Run with `sudo` for system-wide operations
- Check `/etc/paglu/install.conf` for installation details
