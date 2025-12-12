# Smart Home Meta Repository

Repository orchestration using Google Repo tool.

## Installing Repo Tool

### Linux/macOS

```bash
mkdir -p ~/bin
curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
chmod a+x ~/bin/repo
export PATH=~/bin:$PATH
```

Add to your `~/.bashrc` or `~/.zshrc` to make it permanent:
```bash
export PATH=~/bin:$PATH
```

### Ubuntu/Debian

```bash
sudo apt-get install repo
```

## Initializing the Project

Clone and initialize this repository:

```bash
repo init -u https://github.com/kibshh/smart-home-meta.git -b main
```

## Syncing Repositories

After initialization, sync all repositories:

```bash
repo sync
```

To sync a specific project:

```bash
repo sync <project-path>
```

## Common Commands

- **List all projects**: `repo list`
- **Show status**: `repo status`
- **Start a branch**: `repo start <branch-name> --all`
- **Sync all repositories**: `repo sync`
