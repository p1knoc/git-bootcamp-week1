# Mastering Git Log

## Basic Commands
```bash
# Standard log
git log

# One line per commit
git log --oneline

# Last 5 commits
git log -5

# Show actual changes
git log -p

# Commits by specific author
git log --author="Your Name"

# Commits in date range
git log --since="2 days ago"
git log --until="yesterday"
```

## Visual History
```bash
# Graph view (amazing for branches!)
git log --graph --oneline --all

# Even prettier
git log --graph --online --decorate --all

# With dates
git log --graph --oneline --all --date=short --pretty=format:"%h %ad %s"
```

## Search Commits
```bash
# Commits that mention "bug"
git log --grep="bug"

# Commits that changed specific file
git log -- skills.md

# Commits that added/removed "conflict"
git log -S "conflict"
```

## Professional Use Cases

### Finding When BUg Was Introduced
```bash
git log -p -- problematic-file.java
# Read through changes to find the bad commit
```

### Understanding File History
```bash
git log --follow -- renamed-file.md
# Tracks file even through renames
```

### Generating Release Notes
```bash
git log --oneline --since="last release" --grep="feat"
# Lists all feature commits since last release
```

### Code Review Preparation
```bash
git log --stat origin/main..HEAD
# Shows what's different from main branch
```
