# Professional Git Aliases

## My Current Aliases
- `git st` - `git status`
- `git ci` - `git commit`
- `git co` - `git checkout`
- `git lg` - Pretty branch graph `git log --oneline --graph --decorate --all`
- `git last` - Show last commit
- `git unstage <file>` - Unstage files
- `git diffc` - Diff of staged changes
- `git recent` - Show recent branches

## Why Aliases Matter

### Speed
- Senior developers commit ~50 times per day
- Typing "status" 50 times = 300 characters
- Typing "st" 50 times = 100 characters
- Save 200 characters x 250 work days = 50,000 characters/year!

### Muscle Memory
- Consistent shortcuts across projects
- Less context switching
- Faster workflow
- Reduced typos

## Creating Aliases
```bash
git config --global alias.shortcut "full command"
```

## Viewing Aliases
```bash
git config --get-regexp alias
```

## Advanced Alias Examples

### Show what you're about to push
```bash
git config --global alias.ready "diff origin/main..HEAD --stat"
```

### Undo last commit (keep changes)
```bash
git config --global alias.undo "reset --soft HEAD^"
```

### Show who chnaged each line
```bash
git config --global alias.blame "blame -w -C"
```
