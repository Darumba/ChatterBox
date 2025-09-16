
# ChatterBox

An advanced Minecraft chat plugin with channels, moderation, and formatting features for Minecraft 1.21+

## ✨ Features

- **Multi-Channel Chat System** - Global, Local, Admin, and Staff channels
- **Private Messaging** - Send and reply to private messages with /msg and /reply
- **Advanced Moderation** - Mute/unmute players with duration support
- **Anti-Spam Protection** - Prevent message spamming and repetition
- **Word Filtering** - Configurable profanity filter
- **Chat Cooldowns** - Prevent chat flooding
- **Vault Integration** - Support for prefixes and suffixes
- **Permission-Based Channels** - Control channel access with permissions
- **Chat Spy** - Staff can monitor all channel conversations
- **Local Chat** - Location-based chat with configurable range
- **Chat Management** - Clear chat and moderate conversations

## 🎮 Commands

| Command | Description | Permission |
|---------|-------------|------------|
| `/channel [name]` | Switch between channels or view current | `chatterbox.channel.<name>` |
| `/msg <player> <message>` | Send private message | Default |
| `/reply <message>` | Reply to last PM | Default |
| `/mute <player> [duration] [reason]` | Mute a player | `chatterbox.mute` |
| `/unmute <player>` | Unmute a player | `chatterbox.unmute` |
| `/chatclear` | Clear chat for all players | `chatterbox.chatclear` |
| `/chatterbox <reload\|info\|help>` | Main plugin command | `chatterbox.admin` |

### Command Aliases
- `/channel` → `/ch`, `/c`
- `/msg` → `/message`, `/tell`, `/whisper`, `/w`
- `/reply` → `/r`
- `/chatclear` → `/cc`, `/clearchat`
- `/chatterbox` → `/cb`, `/chatbox`

## 🔑 Permissions

### Admin Permissions
- `chatterbox.*` - All permissions
- `chatterbox.admin` - Admin commands (reload, etc.)
- `chatterbox.mute` - Mute players
- `chatterbox.unmute` - Unmute players
- `chatterbox.chatclear` - Clear chat

### Bypass Permissions
- `chatterbox.bypass.*` - Bypass all restrictions
- `chatterbox.bypass.cooldown` - Bypass chat cooldown
- `chatterbox.bypass.spam` - Bypass anti-spam
- `chatterbox.bypass.filter` - Bypass word filter
- `chatterbox.mute.exempt` - Cannot be muted
- `chatterbox.chatclear.bypass` - Don't see clear notifications

### Channel Permissions
- `chatterbox.channel.*` - Access all channels
- `chatterbox.channel.global` - Global channel (default: true)
- `chatterbox.channel.local` - Local channel (default: true) 
- `chatterbox.channel.admin` - Admin channel (default: op)
- `chatterbox.channel.staff` - Staff channel

### Special Permissions
- `chatterbox.spy` - See all channel messages

## 📦 Installation

1. Download the latest release from [Releases](../../releases)
2. Place `ChatterBox.jar` in your `plugins/` folder
3. Restart your server
4. Configure the plugin in `plugins/ChatterBox/config.yml`
5. Install [Vault](https://www.spigotmc.org/resources/vault.34315/) for prefix/suffix support

## ⚙️ Configuration

The plugin creates a comprehensive `config.yml` file with the following sections:

- **Chat Settings** - Format, cooldown, message length
- **Anti-Spam** - Spam protection configuration
- **Word Filter** - Profanity filter settings
- **Channels** - Channel formats and permissions
- **Private Messages** - PM format and sound settings
- **Moderation** - Mute settings and messages
- **Integrations** - Vault, PlaceholderAPI, Discord
- **Advanced** - RGB colors, logging, debug options

## 🔌 Dependencies

### Required
- Minecraft 1.21+
- Java 21+

- [Vault](https://www.spigotmc.org/resources/vault.34315/) - For prefix/suffix support
- [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/) - For placeholder support

## 📸 Screenshots

*Coming soon - Add screenshots of the plugin in action*

## 🐛 Bug Reports & Feature Requests

Please use the [Issues](../../issues) tab to:
- Report bugs
- Request new features  
- Ask questions about usage

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🎯 Roadmap

- [ ] Database support (MySQL, SQLite)
- [ ] Discord webhook integration
- [ ] Chat history and logging
- [ ] Custom channel creation
- [ ] Chat reactions and mentions
- [ ] Multi-language support
- [ ] Web dashboard

## 📞 Support

- **Discord**: *[Discord](https://discord.gg/7H4r8SS8EZ)*
- **Issues**: [GitHub Issues](../../issues)
- **Wiki**: [Plugin Wiki](../../wiki)

## 🙏 Acknowledgments

- Inspired by EssentialsX Chat
- Built for the Minecraft community
- Thanks to all contributors

---

**Version**: 0.0.1  
**Minecraft**: 1.21+  
**Author**: Darumba
