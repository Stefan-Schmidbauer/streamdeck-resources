# Stream Deck Resources

A collection of custom icons, tools, and resources for Elgato Stream Deck.

> **Note:** This is an independent community project and is not affiliated with or endorsed by Elgato.

## Icon Categories

All icons are provided as SVG files (72x72px viewBox) in modern flat design, optimized for dark backgrounds. SVG format ensures universal compatibility - use them directly or convert to PNG as needed (e.g., [OpenDeck](https://github.com/nekename/OpenDeck) automatically converts SVGs to PNGs).

### [ai-work/](ai-work/)
Icons for AI-assisted development workflows (Claude, Cursor, etc.) - number shortcuts, return variations, speech-to-text triggers, and prompt helpers.

### [presentation/](presentation/)
Navigation controls and presentation-specific tools - workspace switching, slide navigation, break indicators.

### [sound/](sound/)
Audio control icons - mute/unmute, volume controls, microphone toggles, and sound settings.

### [system/](system/)
System operations - screen resolution, window management, lock screen, hibernate, screen sharing.

### [workspace/](workspace/)
Workspace/application launcher icons with consistent window design - terminal, IDE, browser, database, chat, and more. See [workspace/workspace-icon-guide.md](workspace/workspace-icon-guide.md) for creating custom workspace icons.

### [misc/](misc/)
Organization and utility icons.

> **For Contributors:** See [icon-style-guide-flat.md](icon-style-guide-flat.md) for design principles and color palette when creating new icons.

## Configuration Examples

Selected examples for [OpenDeck](https://github.com/nekename/OpenDeck) (Linux). Browse the icon folders for more options.

**Requirements:** Some configurations require `xdotool` to be installed (`sudo apt install xdotool` on Debian/Ubuntu).

**Note:** If you experience issues with Input Simulation, all key combinations can alternatively be implemented using `xdotool` via Run Command.

### AI Workflow Examples

| Name | Icon | Action Type | Configuration |
|------|------|-------------|---------------|
| Sinus -> Aa | [speech2text.svg](ai-work/speech2text.svg) | Run Command | Key down: `xdotool keydown ctrl+space`<br>Key up: `xdotool keyup ctrl+space` |
| Return | [return.svg](ai-work/return.svg) | Run Command | Key down: `xdotool key Return` |

## License

MIT License

Copyright (c) 2024 Stefan Schmidbauer

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (including icons and graphics), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Contributing

Feel free to submit your own Stream Deck icons and tools via pull requests!
