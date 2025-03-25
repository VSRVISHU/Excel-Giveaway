# Excel Giveaway Bot 

## Overview
Excel Giveaway is a feature-rich Discord bot designed to create and manage giveaways within Discord servers. It supports customizable giveaways, winner selection, location-based features, and advanced administration tools.

![Excel Giveaway Logo](logo/logo.png)

## Table of Contents
1. [Giveaway Commands](#giveaway-commands)
2. [Utility Commands](#utility-commands) 
3. [Developer Commands](#developer-commands)
4. [Special Features](#special-features)
5. [Getting Started](#getting-started)

## Giveaway Commands
Commands related to creating and managing giveaways.

### /giveaway
Create a new giveaway in the server.

**Options:**
- `prize`: The item or service being given away
- `winners`: Number of winners (default: 1)
- `time`: Duration of the giveaway (e.g., 1d, 12h, 30m)
- `channel`: Channel to host the giveaway in (default: current channel)
- `requirements`: Optional requirements to join the giveaway
- `heatmap`: Enable location tracking for participants (default: disabled)

### /end
End a giveaway early and pick winners.

**Options:**
- `message_id`: ID of the giveaway message to end

### /reroll
Reroll winners for a finished giveaway.

**Options:**
- `message_id`: ID of the giveaway message to reroll
- `winner_count`: Number of new winners to select (default: 1)

### /list
Show all active giveaways in the server.

### /heatmap
Manage the heat map feature for giveaways, showing participant locations.

**Subcommands:**
- `enable`: Enable heat map for a giveaway
- `disable`: Disable heat map for a giveaway
- `view`: View the current heat map for a giveaway

### /countdown
Enable or disable countdown animations for giveaways.

**Options:**
- `giveaway_id`: ID of the specific giveaway 
- `setting`: Enable/disable countdown animations
- `global`: Apply to all giveaways in the server

### /gw-manager
Manage users who can create and manage giveaways.

**Subcommands:**
- `add`: Add a user as a giveaway manager
- `remove`: Remove a user's giveaway manager privileges
- `list`: List all giveaway managers in the server

## Utility Commands

### /help
Display a help menu with all commands organized by category.

### /prefix
View the current bot prefix.

### /prefix-set
Set a new prefix for the bot commands (up to 3 characters).

**Options:**
- `new_prefix`: The new prefix to use for the bot

### /prefix-reset
Reset the bot's prefix to the default.

### /ping
Check the bot's response time and latency.

### /uptime
Check how long the bot has been running.

### /invite
Get an invite link to add the bot to another server.

### /support
Get information about contacting support.

### /botinfo
Display information about the bot and its statistics.

### /set-location
Set your location for giveaways with heat maps.

**Options:**
- `latitude`: Your latitude coordinate
- `longitude`: Your longitude coordinate
- `timezone`: Your timezone (e.g., "Asia/Kolkata")

### /ignore-channel
Set channels where the bot won't respond to commands.

**Subcommands:**
- `add`: Add a channel to the ignored list
- `remove`: Remove a channel from the ignored list
- `list`: Show all currently ignored channels

### /bug-report
Submit a bug report to the bot developers.

**Options:**
- `description`: Detailed description of the bug
- `steps`: Steps to reproduce the bug
- `expected`: What you expected to happen
- `actual`: What actually happened

## Developer Commands
These commands are restricted to the bot owner and development team.

### /blacklist
Manage users blacklisted from using the bot.

**Subcommands:**
- `add`: Add a user to the blacklist
- `remove`: Remove a user from the blacklist
- `check`: Check if a user is blacklisted
- `list`: List all blacklisted users

### /noprefix
Manage users who can use commands without a prefix.

**Subcommands:**
- `add`: Give a user no-prefix permissions
- `remove`: Remove a user's no-prefix permissions
- `list`: List all users with no-prefix permissions

### /noprefixrole
Configure a role that automatically grants no-prefix permissions.

**Subcommands:**
- `create`: Create or set a role for no-prefix permissions
- `disable`: Disable the no-prefix role feature
- `status`: Check the current status of the no-prefix role

### /welcome-dm
Configure welcome DMs sent to new server members.

**Subcommands:**
- `enable`: Enable welcome DMs globally or for a specific server
- `disable`: Disable welcome DMs globally or for a specific server
- `status`: Check the current status of welcome DMs

### /feedback
Send feedback directly to the bot developers.

**Options:**
- `message`: Your feedback message
- `type`: Type of feedback (suggestion, praise, or issue)

### /giveaway-status
Get detailed status information about all giveaways.

## Special Features

### Heat Map
Track and visualize the geographical distribution of giveaway participants with heat maps. This feature allows server administrators to see where their giveaway participants are coming from around the world.

Heat maps can help identify prime times for future giveaways based on participant activity and timezone distribution.

### Custom Prefix
Each server can set its own command prefix for the bot. This allows for better integration with other bots that might use similar prefix patterns.

Prefixes can be up to 3 characters long and can be reset to the default at any time.

### Welcome System
Send customized welcome messages to new members through DMs. These messages can include information about the server, current giveaways, and how to participate.

Welcome DMs can be enabled globally or for specific servers, giving administrators full control over the welcome experience.

### No-Prefix System
Allow specific users or roles to use commands without needing the prefix. This makes the bot more convenient for server staff and giveaway managers.

No-prefix permissions can be granted to individual users or to entire roles, making management flexible and efficient.

### Countdown Animations
Visual countdown animations for giveaways to increase engagement. These animations update the giveaway message with the remaining time, creating excitement as the end approaches.

Countdown animations can be enabled globally or for specific giveaways, depending on the server's preferences.

![Excel Giveaway Banner](logo/banner.png) 

## Getting Started

1. **Invite the Bot**: Use the `/invite` command to get an invite link
2. **Set Permissions**: Make sure the bot has permissions to send messages, embed links, and add reactions
3. **Create a Giveaway**: Use `/giveaway` to create your first giveaway
4. **Set Up Managers**: Use `/gw-manager add` to designate giveaway managers
5. **Customize Settings**: Set your preferred prefix with `/prefix-set`

## Support and Contact

For any questions, issues, or feedback, use the `/support` command or contact the development team through the bot's official support server.
[Join our Support Server](https://discord.gg/puXpZPaCMZ)  

## Recent Updates

### March 25, 2025 - v3 Update 
- Fixed the issue with countdown animations for giveaways
- Improved heatmap functionality and performance
- Enhanced error logging and reporting system
- Optimized bot performance for large servers
- Added new `giveaway-status` command for detailed giveaway analytics

### March 23, 2025 - v2 Update
- Redesigned help menu for better navigation
- Improved bot latency and response time
- Fixed several minor bugs related to giveaway management
- Introduced new role-based permissions for managing giveaways
- Enhanced security for command access

### March 21, 2025 - v1 Update
- Initial release of Excel Giveaway bot
- Implemented core features for creating and managing giveaways
- Added location tracking via heatmap for giveaway participants
- Enabled customizable command prefix for servers
- Introduced welcome DM system for new members
- Bug fixes and minor improvements


*Last updated: March 25, 2025*