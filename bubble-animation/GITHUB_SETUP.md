# GitHub Repository Setup Guide

## Setting up SSH for GitHub

### 1. Generate an SSH key
Open a terminal or Git Bash and run:

```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

Press Enter to accept the default file location. Optionally set a passphrase.

### 2. Start the SSH agent
```bash
eval "$(ssh-agent -s)"
```

### 3. Add your SSH key to the agent
```bash
ssh-add ~/.ssh/id_ed25519
```

### 4. Copy your public SSH key
```bash
# On Windows using Git Bash
cat ~/.ssh/id_ed25519.pub | clip

# On Windows using PowerShell
Get-Content ~/.ssh/id_ed25519.pub | Set-Clipboard
```

### 5. Add the key to GitHub
1. Go to GitHub.com and sign in
2. Click your profile photo in the top right
3. Go to Settings
4. In the left sidebar, click "SSH and GPG keys"
5. Click "New SSH key"
6. Add a descriptive title for your key
7. Paste your key into the "Key" field
8. Click "Add SSH key"

### 6. Test your connection
```bash
ssh -T git@github.com
```
