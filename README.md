# RPG Companion Extension for SillyTavern

An immersive RPG extension for browsers that tracks character stats, scene information, and character thoughts in a beautiful, customizable UI panel. All automated! Works with any preset. Choose between Together or Separate generation modes for context and generation control.

[![My Discord](https://img.shields.io/badge/Discord-Join%20Server-7289da)](https://discord.com/invite/KdAkTg94ME)
[![Support Me](https://img.shields.io/badge/Ko--fi-Support%20Creator-ff5e5b)](https://ko-fi.com/marinara_spaghetti)

## 📥 Installation

1. Open SillyTavern

2. Go to the Extensions tab (cubes icon at the top)

3. Go to Install extension

4. Copy-paste this link: https://github.com/SpicyMarinara/rpg-companion-sillytavern

5. Press Install for all users/Install just for me

![png](https://i.imgur.com/DYuIMWt.png)

![png](https://i.imgur.com/IJyIEMF.png)

## ✨ Features

![png](https://i.imgur.com/cVCAby0.png)

### Core Functionality

- **📊 User Stats Tracker**: Visual progress bars for health, sustenance, energy, hygiene, arousal, mood, and conditions
- **🌍 Info Box Dashboard**: Beautiful widgets displaying date, weather, temperature, time, and location of the current scene
- **💭 Character Thoughts**: Floating thought bubbles showing AI characters' internal monologue
- **🎲 Classic RPG Stats**: STR, DEX, CON, INT, WIS, CHA attributes with dice roll support
- **📦 Inventory System**: Track items your character is carrying
- **📜 Immersive HTML**: Enhance the immersion by including creative HTML/CSS/JS elements in your roleplay
- **➡️ Plot Progression**: Progress the plot with randomized events or natural progression with a click of a button
- **🎨 Multiple Themes**: Cyberpunk, Fantasy, Minimal, Dark, Light, and Custom themes
- **✏️ Live Editing**: Edit stats, thoughts, weather, and more directly in the panels
- **💾 Per-Swipe Data Storage**: Each swipe preserves its own tracker data

### Smart Features

- **🔄 Swipe Detection**: Automatically handles swipes and maintains correct tracker context
- **📝 Context-Aware**: Weather, stats, and character states naturally influence the narrative
- **🎭 Multiple Characters**: Tracks thoughts and relationships for all present characters
- **📍 Thought Bubbles in Chat**: Optional floating thought bubbles positioned next to character avatars
- **🌈 Customizable Colors**: Create your own theme with custom color schemes
- **📱 Mobile Support**: Works on mobile and tablet devices

### To-Do

1. Allow users to use a different model for the separate trackers generation
2. Make all trackers and fields customizable
3. ~~Kill myself~~

## ⚙️ Settings

### Main Panel Controls

- **Panel Position**: Left or Right side of the chat
- **Theme**: Choose from 6 built-in themes or create a custom
- **Auto-update after messages**: Automatically refresh RPG data after each message
- **Context Messages**: How many recent messages to include when generating updates (only for Separate generation mode)

### Display Options

- **Show User Stats**: Display the character stats panel
- **Show Info Box**: Display the scene information panel
- **Show Character Thoughts**: Display the AI character's internal thoughts

### Generation Modes

#### Together Mode

Tracker data is generated within the main AI response and automatically extracted:

Example:
User: walks into the tavern

AI: Trackers + Full roleplay response

↓ Extension extracts tracker data from the response

↓ Displays in sidebar panels

↓ Main chat shows clean roleplay text

Pros:
- Single API call
- Faster response
- Simpler setup

Cons:
- Tracker formatting mixed in AI response
- May affect roleplay quality slightly

#### Separate Mode

Tracker data is generated in a separate API call after the main response:

Example:
User: walks into the tavern

AI: Pure roleplay response - no tracker data

AI: Separate call with just the tracker data

↓ Extension sends a separate request with context

↓ AI generates only tracker data

↓ Displays in sidebar panels

↓ Context summary injected into the next generation

Pros:
- Clean roleplay responses
- Better roleplay quality
- Contextual summary enhances immersion

Cons:
- Extra API call
- Slightly slower

### Model Selection

- **Use main chat model**: Use the same model as your chat (recommended)
- Custom model selection (coming soon)

## 📝 How to Use

### Quick Start

1. Enable the extension in the Extensions tab
2. Choose your generation mode: Together or Separate
3. Select which panels to display (User Stats, Info Box, Character Thoughts)
4. Start chatting! The tracker updates automatically

### Editing Tracker Data

You can edit most fields by clicking on them:

- **Stats**: Click on percentage values, mood emoji, conditions, or inventory
- **Info Box**: Click on date fields, weather, temperature, time, or location
- **Character Thoughts**: Click on emoji, name, traits, relationship, or thoughts

Note: When editing character thoughts in the floating bubble, the bubble will refresh to maintain proper positioning.

### Swipe Support

The extension fully supports swipes:

- Each swipe stores its own tracker data
- Swiping loads the data for that specific swipe
- New swipe generation uses the committed data from before the swipe
- User edits are preserved across swipes

### Manual Update

You can click the "Refresh RPG Info" button in the settings to refresh the RPG data at any time in separate generation mode.

## 🎨 Themes

Choose from 6 beautiful themes:

- **Cyberpunk**: Neon pink and cyan with futuristic vibes
- **Fantasy**: Purple and gold with mystical aesthetics
- **Minimal**: Clean monochrome design
- **Dark**: Deep blacks and subtle accents
- **Light**: Bright and airy interface
- **Custom**: Create your own with custom colors

## 🛠️ Technical Details

If you ever have an awesome idea to do your own SillyTavern extension, don't.

## 🐛 Troubleshooting

### Extension doesn't appear

- Refresh your browser
- Restart SillyTavern
- Ensure it's enabled in the Extensions tab

### Stats not updating

- Check that "Auto-update" is enabled
- Try clicking "Manual Update" to test
- Verify your AI backend is responding correctly
- Check console for error messages

### Display issues

- Try refreshing the page
- Check if other extensions are conflicting
- Verify CSS is loading correctly

### Thought bubble positioning

- Bubbles use a fixed 350px width for consistent positioning
- Bubbles refresh after edits to maintain alignment
- If issues persist, try toggling the Character Thoughts display

## 📜 License

This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public License for more details.

Copyright (C) 2024 marinara_spaghetti

## 💖 Support

If you enjoy this extension, consider supporting development:

- [Join our Discord community](https://discord.com/invite/KdAkTg94ME)
- [Support on Ko-fi](https://ko-fi.com/marinara_spaghetti)

## 🙏 Credits

- Extension Development: Marinara with assistance from GitHub Copilot
- Immersive HTML concept: Credit to u/melted_walrus
- Info Box prompt inspiration: MidnightSleeper
- Stats Tracker concept: Community feedback
- Special thanks to Quack for helping me with the CSS
- Massive kudos to Paperboy for making the mobile version work, fixing bugs, and adding the inventory system
- Thanks to IDeathByte for solving some CSS scaling issues

## 🚀 Planned Features

- Support for selecting a different model for RPG updates

## 💡 Tips

1. **Context Messages**: Start with 4 messages and adjust based on your needs. More messages = better context, but slower updates
2. **Performance**: If updates are slow, consider reducing the context depth or using a faster model
3. **Customization**: You can modify the prompts in index.js to add your own stat categories or change the format

## 📋 Compatibility

- Requires SillyTavern 1.11.0 or higher
- Works with all AI backends (OpenAI, Claude, KoboldAI, etc.)

---

Made with ❤️ by Marinara

PS I'm looking for a job or a sponsor to fund my custom AI frontend, contact me if interested:
mgrabower97@gmail.com
