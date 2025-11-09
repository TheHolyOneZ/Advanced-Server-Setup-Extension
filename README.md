# Advanced-Server-Setup-Extension
The Advanced Server Setup Extension simplifies server creation with pre-configured templates for different needs, like Gaming, Community, Educational, and Business servers, or even a Custom option to build your own. 
> 💡 **Built for the Zygnal Ecosystem — to download and use this extension, you must be part of the Zygnal Ecosystem.**  
> This extension (cog) is part of the **Zygnal Ecosystem** and is only available through its supported platforms.  
> You can use it with:  
> - The **[Discord Bot Framework](https://github.com/TheHolyOneZ/discord-bot-framework)** — ideal for developers who want full control and flexibility *(includes an integrated extension marketplace)*, or  
> - The **[ZygnalBot](https://zygnalbot.de)** — a prebuilt, plug-and-play Discord bot *(also includes an integrated extension marketplace)*.  
>
> Browse and install extensions at [zygnalbot.com/extension](https://zygnalbot.com/extension).  
> For help or community discussions, join us on Discord: [discord.gg/sgZnXca5ts](https://discord.gg/sgZnXca5ts)
# Advanced Server Setup Extension

## Features

### Template Selection
Choose from pre-configured server templates:
- :video_game: **Gaming Server**: Optimized for gaming communities with game-specific channels
- :speech_balloon: **Community Server**: General-purpose community server with social channels
- :books: **Educational Server**: Designed for study groups, classes, and educational communities
- :briefcase: **Business Server**: Professional setup for companies and organizations
- :wrench: **Custom Server**: Start with minimal channels and build your own structure

### Comprehensive Customization
- **Server Naming**: Set a custom name for your server
- **Category Management**: Add, edit, rename, or remove categories
- **Channel Configuration**:
  - Create text and voice channels
  - Set user limits for voice channels
  - Configure announcement channels with proper permissions
- **Template Saving**: Save your server structure as a reusable template

### Interactive UI
- Intuitive button-based navigation
- Dropdown menus for selection
- Modal forms for text input
- Visual progress tracking during setup

## Commands

### `advancedsetup`
**Description**: Starts the interactive server setup wizard
**Usage**: `!advancedsetup`
**Permissions**: Bot Owner only

### `savetemplate`
**Description**: Saves the current server structure as a template
**Usage**: `!savetemplate [template_name]`
**Permissions**: Bot Owner only

## Setup Process

1. **Template Selection**: Choose a base template for your server
2. **Server Naming**: Set a name for your server
3. **Category Customization**: Add, edit, or remove categories and their channels
4. **Confirmation**: Review your setup before applying changes
5. **Setup Completion**: The extension creates all categories and channels according to your configuration

## Technical Details

- Uses Discord's UI components (buttons, selects, modals) for interactive setup
- Maintains session state to track setup progress
- Handles rate limiting during channel creation
- Provides detailed error messages for troubleshooting

## Requirements

- Discord.py 2.0+ (with UI components support)
- Bot must have "Manage Channels" and "Manage Guild" permissions in the server

## Notes

- The setup process modifies the existing server where the command is used
- Large server setups may take some time due to Discord's rate limiting
- Templates can be expanded by modifying the `templates` dictionary in the code
