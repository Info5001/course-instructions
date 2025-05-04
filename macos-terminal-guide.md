# macOS Terminal Guide with Oh My Zsh

This guide will help you set up and effectively use the Terminal application on macOS with Oh My Zsh for an improved command-line experience.

## Getting Started with Terminal

### Opening Terminal

1. Click on the **Spotlight** search icon (magnifying glass) in the top-right corner of your screen
2. Type `Terminal` and press **Enter**
3. Alternatively, navigate to **Applications** > **Utilities** > **Terminal**

### Basic Terminal Commands

| Command   | Description                                | Example                                     |
| --------- | ------------------------------------------ | ------------------------------------------- |
| `pwd`     | Print working directory (current location) | `pwd`                                       |
| `ls`      | List files and directories                 | `ls -la` (show all files with details)      |
| `cd`      | Change directory                           | `cd Documents` or `cd ..` (go up one level) |
| `mkdir`   | Create a new directory                     | `mkdir projects`                            |
| `rm`      | Remove files                               | `rm filename.txt`                           |
| `rmdir`   | Remove empty directory                     | `rmdir emptydir`                            |
| `touch`   | Create an empty file                       | `touch newfile.txt`                         |
| `cp`      | Copy files                                 | `cp file.txt Documents/`                    |
| `mv`      | Move or rename files                       | `mv file.txt newname.txt`                   |
| `cat`     | Display file contents                      | `cat file.txt`                              |
| `clear`   | Clear terminal screen                      | `clear`                                     |
| `history` | Show command history                       | `history`                                   |

## Setting Up Oh My Zsh

Oh My Zsh is an open-source framework for managing your Zsh configuration that comes with helpful functions, plugins, themes, and more.

### Prerequisites

1. Make sure you have **Zsh** installed (default shell in macOS Catalina and newer):

   ```bash
   zsh --version
   ```

2. Install **Homebrew** if you don't have it:
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

### Installing Oh My Zsh

1. Install Oh My Zsh using curl:

   ```bash
   sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
   ```

2. After installation, your terminal will automatically restart with Oh My Zsh active

### Customizing Oh My Zsh

1. **Edit your configuration file**:

   ```bash
   nano ~/.zshrc
   ```

2. **Change the theme** by modifying the `ZSH_THEME` line:

   ```bash
   # Popular themes: robbyrussell, agnoster, avit, bira
   ZSH_THEME="robbyrussell"
   ```

3. **Add plugins** by modifying the `plugins` line:

   ```bash
   plugins=(git vscode brew macos)
   ```

4. Save changes and apply them:
   ```bash
   source ~/.zshrc
   ```

### Popular Oh My Zsh Plugins

- **git**: Provides aliases and functions for Git
- **vscode**: Adds commands to open VS Code
- **brew**: Adds completion for Homebrew commands
- **macos**: Provides macOS-specific commands
- **z**: Quickly jump between directories using 'frecency'

## Terminal Productivity Tips

### Command Shortcuts

- **Up/Down arrows**: Navigate through command history
- **Ctrl+A**: Move cursor to beginning of line
- **Ctrl+E**: Move cursor to end of line
- **Ctrl+U**: Clear line before cursor
- **Ctrl+K**: Clear line after cursor
- **Ctrl+R**: Search command history
- **Tab**: Auto-complete commands and file paths

### Creating Aliases

Add custom shortcuts by editing your `~/.zshrc` file:

```bash
# Example aliases
alias gs="git status"
alias gc="git commit -m"
alias ll="ls -la"
```

### Environment Variables

To add permanent environment variables:

1. Edit your `~/.zshrc` file:

   ```bash
   nano ~/.zshrc
   ```

2. Add export statements:

   ```bash
   export JAVA_HOME=$(/usr/libexec/java_home)
   export PATH=$PATH:$JAVA_HOME/bin
   ```

3. Apply changes:
   ```bash
   source ~/.zshrc
   ```

## Additional Resources

- [Oh My Zsh Documentation](https://github.com/ohmyzsh/ohmyzsh/wiki)
- [Terminal User Guide for Mac](https://support.apple.com/guide/terminal/welcome/mac)
- [Zsh Documentation](http://zsh.sourceforge.net/Doc/)

---

Last updated: May 4, 2025
