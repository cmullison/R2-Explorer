🔄 Your New Development Workflow
Now when you want to make style changes:

1. Edit the Dashboard Source Code

# Make your style changes in:

packages/dashboard/src/

2. Rebuild and Update Template

pnpm run build-dashboard # Build your changes
pnpm run build-worker # Copy dashboard to worker package
cd template && npm install

3. Test Your Changes

cd template
pnpm dev # or npm run dev

🎨 Where to Make Style Changes

The dashboard uses Quasar Framework (Vue.js), so you can edit:

CSS files: packages/dashboard/src/css/
Component styles: packages/dashboard/src/components/
Layout styles: packages/dashboard/src/layouts/

<div align="center">
  <a href="https://r2explorer.com/">
    <img src="https://raw.githubusercontent.com/G4brym/R2-explorer/refs/heads/main/packages/docs/pages/assets/r2-explorer-logo.png" width="500" height="auto" alt="R2-Explorer"/>
  </a>
</div>

<p align="center">
    <em>A Google Drive Interface for your Cloudflare R2 Buckets!</em>
</p>

<p align="center">
    <a href="https://github.com/G4brym/R2-Explorer/commits/main" target="_blank">
      <img src="https://img.shields.io/github/commit-activity/m/G4brym/R2-Explorer?label=Commits&style=social" alt="R2-Explorer Commits">
    </a>
    <a href="https://github.com/G4brym/R2-Explorer/issues" target="_blank">
      <img src="https://img.shields.io/github/issues/G4brym/R2-Explorer?style=social" alt="Issues">
    </a>
    <a href="https://github.com/G4brym/R2-Explorer/blob/main/LICENSE" target="_blank">
      <img src="https://img.shields.io/badge/license-MIT-brightgreen.svg?style=social" alt="Software License">
    </a>
</p>

# R2-Explorer

R2-Explorer brings a familiar Google Drive-like interface to your Cloudflare R2 storage buckets, making file management simple and intuitive.

## Quick Links

- 📚 **Documentation**: [r2explorer.com](https://r2explorer.com)
- 🎮 **Live Demo**: [demo.r2explorer.com](https://demo.r2explorer.com)
- 💻 **Source Code**: [github.com/G4brym/R2-Explorer](https://github.com/G4brym/R2-Explorer)

Available in multiple languages:
[English](https://r2explorer.com) |
[Español](https://r2explorer-com.translate.goog/?_x_tr_sl=en&_x_tr_tl=es) |
[Português](https://r2explorer-com.translate.goog/?_x_tr_sl=en&_x_tr_tl=pt-PT) |
[Français](https://r2explorer-com.translate.goog/?_x_tr_sl=en&_x_tr_tl=fr)

## Overview

R2-Explorer transforms your Cloudflare R2 storage experience with a modern, user-friendly interface. It provides powerful file management capabilities while maintaining enterprise-grade security through Cloudflare's infrastructure.

## Key Features

- **🔒 Security**

  - Basic Authentication support
  - Cloudflare Access integration
  - Self-hosted on your Cloudflare account

- **📁 File Management**

  - Drag-and-drop file upload
  - Folder creation and organization
  - Multi-part upload for large files
  - Right-click context menu for advanced options
  - HTTP/Custom metadata editing

- **👀 File Handling**

  - In-browser file preview
    - PDF documents
    - Images
    - Text files
    - Markdown
    - CSV
    - Logpush files
  - In-browser file editing
  - Folder upload support

- **📧 Email Integration**
  - Receive and process emails via Cloudflare Email Routing
  - View email attachments directly in the interface

## Installation Methods

Choose the method that best suits your needs:

1. **GitHub Action (Recommended)**

   [Follow the guide here](https://r2explorer.com/getting-started/creating-a-new-project/#1st-method-github-action-recommended)

2. **Cloudflare CLI**

   [Follow the guide here](https://r2explorer.com/getting-started/creating-a-new-project/#2nd-method-create-cloudflare)

3. **Template Repository**

   [Use our template here](https://github.com/G4brym/R2-Explorer/tree/main/template)

For detailed instructions on maintaining and updating your installation, visit our [update guide](https://r2explorer.com/getting-started/updating-your-project/).

## Roadmap

We're actively working on these exciting features:

- **File Management**

  - Support for bucket names with spaces
  - File search functionality
  - Folder renaming capability
  - Image thumbnails generation

- **AI Integration**

  - Object detection using workers-ai

- **User Experience**
  - Enhanced timestamp tooltips
  - Email response capabilities
  - Advanced file type-specific editing

## Known Issues

- When using basic authentication, email inline images and assets don't load properly
- Additional issues can be found and reported on our [GitHub Issues](https://github.com/G4brym/R2-Explorer/issues) page

## Contributing

We welcome contributions! Whether it's bug fixes, new features, or documentation improvements, please feel free to:

1. Fork the repository
2. Create a feature branch
3. Submit a Pull Request

## Support

- 📚 Documentation: [r2explorer.com](https://r2explorer.com)
- 🐛 Issue Tracker: [GitHub Issues](https://github.com/G4brym/R2-Explorer/issues)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
