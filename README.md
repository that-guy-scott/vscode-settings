# VS Code Settings

Personal VS Code configuration with Vim navigation, IntelliJ-style global shortcuts, and Codex integration.

## Files

- `settings.json` — editor settings, Vim configuration, and leader mappings
- `keybindings.json` — global keyboard shortcuts
- `extensions.txt` — saved extension list for bulk installation

## Editor Settings

| Setting | Value |
|---------|-------|
| Font | DroidSansM Nerd Font |
| Font Size | 16 |
| UI Zoom | 0.8 |
| Color Theme | Dark Modern |
| Line Numbers | Relative |
| Font Ligatures | Enabled |
| Format on Save | Enabled |
| Auto Save | After Delay |
| Cursor Animation | Smooth |
| Sticky Scroll | Disabled |
| Editor Tabs | Hidden |
| Activity Bar | Hidden |
| Menu Bar | Compact |

## Vim Configuration

**Leader key:** `;`

Leader mappings are available in Vim Normal mode.

### Views

| Key | Action |
|-----|--------|
| `;1` | File Explorer |
| `;2` | Bookmarks |
| `;3` | Todo Tree |
| `;4` | Problems |
| `;5` | Source Control |
| `;6` | Testing |
| `;7` | Outline |
| `;8` | Zen Mode |

### Codex

| Key | Action |
|-----|--------|
| `;cc` | Focus Codex |
| `;cn` | Start a new chat |
| `;ca` | Add the current selection to the thread |
| `;cf` | Add the current file to the thread |
| `;cp` | Open a new Codex agent panel |

The Codex mappings require the OpenAI extension (`openai.chatgpt`).

### Top Row

| Key | Action |
|-----|--------|
| `;q`, `;Q` | Show Hover |
| `;w`, `;F`, `;g`, `;m` | Go to Symbol in File |
| `;W` | Save File |
| `;e`, `;s`, `;sf`, `;ff` | Quick Open |
| `;E`, `;R` | Recent Editors |
| `;r` | Run Without Debugging |
| `;t` | Toggle Terminal |
| `;T` | Focus Terminal |
| `;u` | Half Page Up |
| `;i` | Toggle Bookmark |
| `;o` | Open File |
| `;p` | Navigate Back |
| `;P` | Toggle Zen Mode |

### Middle Row

| Key | Action |
|-----|--------|
| `;Esc` | Close Panel and Sidebar |
| `;a` | Command Palette |
| `;A` | Select All |
| `;sr` | Open Recent |
| `;d` | Half Page Down |
| `;dd` | New Untitled File |
| `;D` | Open Current File's Git Diff |
| `;f` | Find in Files |
| `;h` | Toggle Line Comment |
| `;H` | Split Editor Down |
| `;j` | Next Bookmark |
| `;k` | Previous Bookmark |
| `;l`, `;;` | Last Edit Location |

### Bottom Row

| Key | Action |
|-----|--------|
| `;z` | Quick Fix |
| `;x` | Close All Editors |
| `;v` | Select Inner WORD |
| `;V` | Split Editor Right |
| `;b` | Jump to Matching Bracket |
| `;n` | Next Editor |
| `;M` | Go to Symbol in Workspace |
| `;.` | Toggle Breakpoint |
| `;/` | Clear Search Highlight |

### Navigation and Goto

| Key | Action |
|-----|--------|
| `]d` | Next Diagnostic |
| `[d` | Previous Diagnostic |
| `ge` | Command Palette |
| `gu` | Find References |
| `gi` | Go to Implementation |
| `gh` | Open Local History |
| `Y` | Yank to End of Line |
| `U` | Redo |

### Visual Mode

| Key | Action |
|-----|--------|
| `;h` | Toggle Line Comment |
| `;f` | Find in Files |
| `;i` | Start Inline Chat |

## Global Keybindings

These shortcuts work outside Vim leader handling unless a `when` condition limits them.

### Focus and Navigation

| Key | Action |
|-----|--------|
| `Escape` | Return focus to the active editor |
| `Shift+Escape` | Close sidebars and panels, then focus the editor |
| `Ctrl+Shift+I` | Focus Codex |
| `Ctrl+Shift+N`, `Ctrl+E` | Quick Open |
| `Ctrl+Shift+E` | Recent Editors |
| `Shift Shift`, `Ctrl+Shift+A` | Command Palette |
| `Ctrl+Alt+Left` | Navigate Back |
| `Ctrl+Alt+Right` | Navigate Forward |
| `Ctrl+Alt+B` | Toggle Auxiliary Bar |
| `Ctrl+Tab` | Previous/Next Recently Used Editor |
| `Ctrl+Shift+Tab` | Reverse Recently Used Editor Navigation |
| `Ctrl+Shift+F12` | Toggle Maximized Panel |

### Code Navigation and Refactoring

| Key | Action |
|-----|--------|
| `Alt+Home` | Focus Breadcrumbs |
| `Alt+F7` | Find References |
| `Ctrl+F12` | Go to Symbol |
| `Shift+F6` | Rename |
| `Alt+Insert` | Source Actions |
| `Ctrl+Alt+Shift+T` | Refactor |
| `Ctrl+Alt+V` | Refactor |
| `Ctrl+Alt+M` | Refactor |

### Editing

| Key | Action |
|-----|--------|
| `Ctrl+D` | Duplicate Selection in Insert mode |
| `Ctrl+Y` | Delete Line in Normal mode |
| `Ctrl+Shift+Up/Down` | Move Lines |
| `Ctrl+W` | Expand Selection |
| `Ctrl+Shift+W` | Close Active Editor |
| `Ctrl+Alt+L` | Format Document |
| `Ctrl+Alt+O` | Organize Imports |

### Search

| Key | Action |
|-----|--------|
| `Ctrl+F` | Find in Insert mode |
| `Ctrl+H` | Replace in Files |
| `Ctrl+Shift+F` | Find in Files |
| `Ctrl+Shift+R` | Replace in Files |

### Run and Debug

| Key | Action |
|-----|--------|
| `Shift+F10` | Run Without Debugging |
| `Shift+F9` | Start Debugging |
| `Ctrl+F2` | Stop Debugging |
| `F8` | Continue |
| `F7` | Step Into |

### Tool Windows

| Key | Action |
|-----|--------|
| `Alt+0` | Toggle Claude Sidebar |
| `Alt+1` | Toggle File Explorer |
| `Alt+2` | Bookmarks |
| `Alt+3` | Find in Files |
| `Alt+4` | Run Without Debugging |
| `Alt+5` | Debug View |
| `Alt+7` | Outline |
| `Alt+9` | Source Control |
| `Alt+F12` | Toggle Terminal |

### Bookmarks and Git

| Key | Action |
|-----|--------|
| `F11` | Toggle Bookmark |
| `Shift+F11` | List Bookmarks |
| `Ctrl+K` | Commit Staged Changes when the editor is not focused |

## Installation

### Settings and Keybindings

This machine uses symlinks so edits in the repository are applied directly:

```bash
ln -s /path/to/vscode-settings/settings.json ~/.config/Code/User/settings.json
ln -s /path/to/vscode-settings/keybindings.json ~/.config/Code/User/keybindings.json
```

Alternatively, copy the files into the VS Code user settings directory.

**Linux:**

```bash
cp settings.json keybindings.json ~/.config/Code/User/
```

**macOS:**

```bash
cp settings.json keybindings.json ~/Library/Application\ Support/Code/User/
```

**Windows:**

```powershell
copy settings.json keybindings.json %APPDATA%\Code\User\
```

### Extensions

Review `extensions.txt`, then install its entries:

```bash
xargs -L 1 code --install-extension < extensions.txt
```

Refresh the extension snapshot with:

```bash
code --list-extensions > extensions.txt
```
