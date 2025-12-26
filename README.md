# Zap! ⚡

a dangerous writing plugin for Obsidian, inspired by the [Most Dangerous Writing App](https://www.squibler.io/dangerous-writing-prompt-app). run timed or word-goal writing sprints and keep typing—if you stop for more than 5 seconds, your content gets deleted (_zapped_)! ⏱️

## Features

- **Timed Writing Sessions**: Set a duration for your writing session.
- **Word Count Goals**: Target a specific word count instead of a timer.
- **Idle Detection**: Stop typing for 5 seconds (configurable) and face the penalty.
- **Penalty Options**: Choose to delete entire file, last paragraph, or just last sentence.
- **Visual Warnings**: Progressive colored overlay warns you as idle time approaches.
- **Custom Warning Color**: Pick your own warning color in settings.
- **Status Bar**: Shows remaining session time and idle countdown.
- **Practice Mode**: Enabled by default - recover content after a penalty.
- **Statistics Dashboard**: Track your writing history with stats for today, past week, month, and all time.

## Installation

### From Community Plugins

1. Open Obsidian Settings → Community plugins
2. Search for "Zap"
3. Click Install, then Enable

### Manual Installation

1. Download `main.js`, `manifest.json`, and `styles.css` from the latest release.
2. Create a folder called `zap-writing` in your vault's `.obsidian/plugins/` directory.
3. Copy the downloaded files into this folder.
4. Reload Obsidian and enable the plugin in Settings → Community plugins.

## Usage

1. Open a Markdown file in Obsidian.
2. Click the zap icon (⚡) in the ribbon, or use command palette: "Start Zap writing session".
3. Configure a time or word goal and click "Start Zap Session".
4. Keep typing! If you stop for more than 5 seconds, content is deleted.
5. Complete the session to keep your content.

## Settings

| Setting           | Description                                                      | Default       |
| ----------------- | ---------------------------------------------------------------- | ------------- |
| Session duration  | How long each writing session lasts                              | 5 minutes     |
| Word count goal   | Default words to target when using word mode                     | 0 (disabled)  |
| Idle timeout      | How long you can stop before penalty                             | 5 seconds     |
| Penalty type      | What gets deleted: entire file, last paragraph, or last sentence | Entire file   |
| Practice mode     | Enable to recover content after a penalty                        | On            |
| Warning threshold | How long idle before visual warnings start                       | 1.5 seconds   |
| Warning color     | Color of the warning overlay                                     | Red (#ff0000) |

## Statistics

Open the statistics view via:

- Command palette: "Open writing statistics"
- Settings → Statistics → View All Stats

View your writing history including:

- Total sessions, completed sessions, words written, time spent
- Stats for Today, Past Week, Past Month, and All Time
- Recent session history with completion status

## Commands

- `Start Zap writing session` - Begin a new session.
- `Stop Zap writing session` - End the current session early.
- `Open writing statistics` - View your Zap writing stats.

## Safety Notes

⚠️ **Practice mode is ON by default** - you can always recover content after a penalty.

- Always test in a safe vault first.
- The plugin tracks the active file - switching files ends the session.
- Make backups before disabling practice mode.
- Click any completion/penalty notice to dismiss it.

## License

This plugin is licensed under the [MIT License](LICENSE).
