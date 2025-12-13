# Stream Deck Resources

A collection of custom icons, tools, and resources for Elgato Stream Deck.

> **Note:** This is an independent community project and is not affiliated with or endorsed by Elgato.

## Icons and Configuration

AI-generated icons designed for Stream Deck buttons, optimized for 72x72px button size and work well on both light and dark themes.

### Configuration Examples

Suggested button configurations for OpenDeck (Linux).

**Requirements:** Some configurations require `xdotool` to be installed (`sudo apt install xdotool` on Debian/Ubuntu).

**Note:** If you experience issues with Input Simulation, all key combinations can alternatively be implemented using `xdotool` via Run Command (e.g., `xdotool key 1` instead of `[Text("1")]`).

| Name | Icon | Action Type | Configuration |
|------|------|-------------|---------------|
| 1 | **number-1.svg** | Input Simulation | `[Text("1")]` |
| 2 | **number-2.svg** | Input Simulation | `[Text("2")]` |
| 3 | **number-3.svg** | Input Simulation | `[Text("3")]` |
| 4 | **number-4.svg** | Input Simulation | `[Text("4")]` |
| tell what to do | **tell-what-to-do.svg** | Input Simulation | `[Key(UpArrow, Click)]` |
| Sinus -> Aa | **speech2text.svg** | Input Simulation | Key down: `[Key(Control, Press), Key(Space, Press)]`<br>Key up: `[Key(Space, Release), Key(Control, Release)]` |
| Sinus -> Aa + Return | **speech2text-return.svg** | Run Command | Key down: `xdotool keydown ctrl+space`<br>Key up: `xdotool keyup ctrl+space && sleep 1 && xdotool key Return` |
| Return | **return.svg** | Input Simulation | Key down: `[Key(Return, Click)]` |
| Shift + Return | **shift-return.svg** | Input Simulation | Key down: `[Key(Shift, Press), Key(Return, Click), Key(Shift, Release)]` |
| Alt + Return | **alt-return.svg** | Input Simulation | Key down: `[Key(Alt, Press), Key(Return, Click), Key(Alt, Release)]` |

_Note: These configurations are optimized for OpenDeck on Linux. Adjust to fit your workflow and software._

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
