# VS Code Settings

Personal VS Code configuration with Vim keybindings and IntelliJ-style shortcuts.

## Files

- `settings.json` - Editor settings, Vim configuration, and leader key mappings
- `keybindings.json` - Global keyboard shortcuts (IntelliJ-style)

## Editor Settings

| Setting | Value |
|---------|-------|
| Font | DroidSansM Nerd Font |
| Font Size | 14 |
| Line Numbers | Relative |
| Font Ligatures | Enabled |
| Format on Save | Enabled |
| Auto Save | After Delay |
| Cursor Animation | Smooth |
| Sticky Scroll | Disabled |

## Vim Configuration

**Leader Key:** `;`

### Normal Mode - Leader Mappings

#### Number Row (Sidebar/Views)
| Key | Action |
|-----|--------|
| `;1` | File Explorer |
| `;2` | Bookmarks View |
| `;3` | Todo Tree View |
| `;7` | Outline |
| `;8` | Zen Mode |

#### Top Row
| Key | Action |
|-----|--------|
| `;q` | Show Hover |
| `;w` | Go to Symbol in File |
| `;W` | Save File |
| `;e` | Quick Open |
| `;E` | Recent Editors |
| `;r` | Run (Debug) |
| `;t` | Toggle Terminal |
| `;u` | Half Page Up |
| `;i` | Toggle Bookmark |
| `;o` | Open File |
| `;p` | Navigate Back |
| `;P` | Zen Mode |

#### Middle Row
| Key | Action |
|-----|--------|
| `;Esc` | Close Panel & Sidebar |
| `;a` | Command Palette |
| `;A` | Select All |
| `;s` | Quick Open |
| `;sr` | Open Recent |
| `;sf` | Quick Open |
| `;d` | Half Page Down |
| `;dd` | New Untitled File |
| `;f` | Find in Files |
| `;ff` | Quick Open |
| `;F` | Go to Symbol |
| `;g` | Go to Symbol |
| `;h` | Toggle Comment |
| `;H` | Split Editor Down |
| `;j` | Jump to Next Bookmark |
| `;k` | Jump to Previous Bookmark |
| `;l` | Last Edit Location |
| `;;` | Last Edit Location |

#### Bottom Row
| Key | Action |
|-----|--------|
| `;x` | Close All Editors |
| `;v` | Select Inner WORD |
| `;V` | Split Editor Right |
| `;b` | Jump to Matching Bracket |
| `;B` | Bookmarks View |
| `;n` | Next Editor |
| `;m` | Go to Symbol |
| `;M` | Go to Symbol (Workspace) |
| `;.` | Toggle Breakpoint |
| `;/` | Clear Search Highlight |

#### Goto Commands
| Key | Action |
|-----|--------|
| `ge` | Command Palette |
| `gu` | Find References |
| `gi` | Go to Implementation |
| `gh` | Open Local History |

#### Navigation
| Key | Action |
|-----|--------|
| `]]` | Next Problem |
| `[[` | Previous Problem |
| `Y` | Yank to End of Line |
| `U` | Redo |

### Visual Mode - Leader Mappings
| Key | Action |
|-----|--------|
| `;h` | Toggle Comment |
| `;f` | Find in Files |

## Global Keybindings (IntelliJ-Style)

### Navigation
| Key | Action |
|-----|--------|
| `Ctrl+N` | Quick Open |
| `Ctrl+Shift+N` | Quick Open |
| `Ctrl+E` | Quick Open |
| `Ctrl+Shift+E` | Recent Editors |
| `Ctrl+Alt+Left` | Navigate Back |
| `Ctrl+Alt+Right` | Navigate Forward |
| `Ctrl+Tab` | Previous Editor in Group |
| `Ctrl+Shift+Tab` | Least Recent Editor |

### Code Navigation
| Key | Action |
|-----|--------|
| `Ctrl+B` | Go to Definition |
| `Ctrl+Alt+B` | Go to Implementation |
| `Alt+F7` | Find References |
| `Ctrl+F12` | Go to Symbol |

### Refactoring
| Key | Action |
|-----|--------|
| `Shift+F6` | Rename |
| `Ctrl+Alt+Shift+T` | Refactor |
| `Ctrl+Alt+V` | Refactor |
| `Ctrl+Alt+M` | Refactor |

### Editing
| Key | Action |
|-----|--------|
| `Ctrl+D` | Duplicate Selection (Insert mode) |
| `Ctrl+Y` | Delete Line (Normal mode) |
| `Ctrl+Shift+Up/Down` | Move Lines |
| `Ctrl+W` | Expand Selection |
| `Ctrl+Shift+W` | Close Editor |
| `Ctrl+Alt+L` | Format Document |
| `Ctrl+Alt+O` | Organize Imports |

### Search
| Key | Action |
|-----|--------|
| `Ctrl+F` | Find (Insert mode) |
| `Ctrl+H` | Replace in Files |
| `Ctrl+Shift+F` | Find in Files |
| `Ctrl+Shift+R` | Replace in Files |
| `Ctrl+Shift+A` | Command Palette |

### Run/Debug
| Key | Action |
|-----|--------|
| `Shift+F10` | Run |
| `Shift+F9` | Debug |
| `Ctrl+F2` | Stop |
| `F8` | Continue |
| `F7` | Step Into |

### Tool Windows (Alt+Number)
| Key | Action |
|-----|--------|
| `Alt+1` | Toggle Sidebar |
| `Alt+2` | Bookmarks |
| `Alt+3` | Find in Files |
| `Alt+4` | Run |
| `Alt+5` | Debug View |
| `Alt+7` | Outline |
| `Alt+9` | Source Control |
| `Alt+F12` | Terminal |

### Bookmarks
| Key | Action |
|-----|--------|
| `F11` | Toggle Bookmark |
| `Shift+F11` | List Bookmarks |

### Git
| Key | Action |
|-----|--------|
| `Ctrl+K` | Commit Staged |

## Installation

Copy files to your VS Code user settings directory:

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

## Required Extensions

- [Vim](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim)
- [Bookmarks](https://marketplace.visualstudio.com/items?itemName=alefragnani.Bookmarks)
- [Todo Tree](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree)
