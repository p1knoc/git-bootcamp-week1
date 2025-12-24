# Repository Maintenace Guide

## Daily Hygiene
- Commit frequently (at least 3-5 times per day)
- Write clear commit messages
- Pull from main before starting work
- Push at end of day

## Weekly Tasks
- Review and clean up branches
- Update documentation
- Check .gitignore is working
- Review commit history for issues

## Monthly Tasks
- Clean up old merged branches
- Update dependencies
- Review repository size
- Archive completed features

## Commands for Maintenance

### See All Branches (Local and Remote)
```bash
git brnach -a
```

### Delete Old Local Branches
```bash
# Delete specific branch
git branch -d branch-name

# Delete all merged branches
git branch --merged | grep -v "main" | xargs git branch -d
```

### Check Repository Size
```bash
du -sh .git
```

### See Largest Files in History
```bash
git rev-list --objects --all | \
    git cat-file --batch-check='%(objecttype) %(objectname) %(objectsize) %(rest) | \
    grep '^blob' | \
    sort -k3 -n -r | \
    head -10
```

### Clean Up Repository
```bash
# Remove untracked files (be careful!)
git clean -n # Dry run first
git clean -f # Actually remove

# Clean up tracking branches
git fetch --prune
```

## Red Flags
- Repository over 1GB (without good reason)
- Hundreds of unmerged branches
- Build artifacts in history
- Sensitive data committed
- No commits in days (on active project)

## Professional Standards
- Keep main branch always deployable
- Feature branches < 3 days old
- Clear commit messages
- No merge commits without reason
- Regular documentation updates
