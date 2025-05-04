# Windows Terminal Guide with Git Bash and Oh My Zsh

This guide will help you set up and effectively use Windows Terminal with Git Bash and Oh My Zsh for an improved command-line experience.

## Setting Up Windows Terminal

Windows Terminal is a modern terminal application that allows you to use multiple command-line tools in tabs.

### Installation

1. **Microsoft Store Method** (Recommended):

   - Open the **Microsoft Store** from the Start menu
   - Search for **Windows Terminal**
   - Click **Get** or **Install**

2. **Manual Installation**:
   - Visit [Windows Terminal GitHub Releases](https://github.com/microsoft/terminal/releases)
   - Download the latest `.msixbundle` file
   - Double-click to install

### Configuration

1. Open Windows Terminal (you'll see PowerShell as the default profile)
2. Click the dropdown arrow next to the "+" tab and select **Settings**
3. This opens a JSON file where you can customize terminal settings:
   - Set the default profile
   - Add new profiles
   - Change color schemes
   - Adjust keyboard shortcuts

## Setting Up Git Bash in Windows Terminal

### Prerequisites

1. Install **Git for Windows** if not already installed:
   - Download from [Git for Windows](https://gitforwindows.org/)
   - During installation, choose "Use Git from Git Bash only" or "Use Git from Windows Command Prompt"
   - Accept other default options

### Add Git Bash to Windows Terminal

Git Bash should automatically appear as a profile in Windows Terminal after installation. If not:

1. Open Windows Terminal settings (Ctrl+,)
2. Click "Add a new profile" → "New empty profile"
3. Configure these settings:

   - **Name**: Git Bash
   - **Command line**: `C:\Program Files\Git\bin\bash.exe` (adjust if your installation path differs)
   - **Starting directory**: `%USERPROFILE%`
   - **Icon**: `C:\Program Files\Git\mingw64\share\git\git-for-windows.ico`

4. Set Git Bash as default (optional):
   - Find the GUID for Git Bash under "profiles"
   - Copy this GUID
   - Paste it as the value for "defaultProfile" at the top of the settings file

## Basic Git Bash Commands

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

## Setting Up Oh My Zsh in Git Bash

While Git Bash uses Bash by default, you can enhance your experience with Oh My Zsh by installing Zsh.

### Installing Zsh in Git Bash

1. **Using Git Bash Package Manager**:

   ```bash
   # Update package lists
   pacman -Syu

   # Install zsh
   pacman -S zsh
   ```

2. **Alternative Method** (if pacman doesn't work):

   - Download the [Zsh for Windows](https://packages.msys2.org/package/zsh?repo=msys&variant=x86_64) package
   - Extract to your Git installation directory (e.g., `C:\Program Files\Git`)

3. **Set Zsh as default shell**:
   ```bash
   # Add this to your ~/.bashrc file
   if [ -t 1 ]; then
     exec zsh
   fi
   ```

### Installing Oh My Zsh

1. Install Oh My Zsh using curl:

   ```bash
   sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
   ```

2. After installation, restart Git Bash to apply changes

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
   plugins=(git vscode)
   ```

4. Save changes and apply them:
   ```bash
   source ~/.zshrc
   ```

### Popular Oh My Zsh Plugins

- **git**: Provides aliases and functions for Git
- **vscode**: Adds commands to open VS Code
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
   export JAVA_HOME="/c/Program Files/Amazon Corretto/jdk17.x.x_x"
   export PATH=$PATH:$JAVA_HOME/bin
   ```

3. Apply changes:
   ```bash
   source ~/.zshrc
   ```

## Troubleshooting

### Common Issues

1. **"Command not found" errors**:

   - Ensure the command is installed and in your PATH
   - For Git commands, verify Git is properly installed

2. **Permission issues**:

   - Use "Run as Administrator" if needed
   - Check file permissions with `ls -la`

3. **Path issues**:
   - Use proper path syntax (forward slashes or escaped backslashes)
   - For Windows paths, use `/c/Users/...` instead of `C:\Users\...`

### Windows-Specific Tips

1. **Accessing Windows drives**:

   - Windows drives are mounted under `/c`, `/d`, etc.
   - Example: `cd /c/Users/username/Documents`

2. **Running Windows commands**:
   - To run Windows executable commands, use a `.exe` suffix
   - Example: `notepad.exe file.txt`

## Additional Resources

- [Windows Terminal Documentation](https://docs.microsoft.com/en-us/windows/terminal/)
- [Git Bash Documentation](https://git-scm.com/book/en/v2)
- [Oh My Zsh Documentation](https://github.com/ohmyzsh/ohmyzsh/wiki)

---

Last updated: May 4, 2025
