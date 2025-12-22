# Conflict Prevention Strategies

## Communication
- Tell team which files you're working on
- Use Slack/Discord to coordinate
- Small, focused branches reduce conflicts

## Technical Practices
- Pull from main frequently ('git pull origin main')
- Merge main into your feature branch regularly
- Keep branches short-lived (< 3 days)
- Use feature flags for long-running features

## When Conflicts Happen
1. Don't panic - conflicts are normal
2. Read the conflict markers carefully
3. Communicate with the other developer
4. Test after resolving
5. Commit with clear merge message

## Tools That Help
- 'git diff' - See exactly what changed
- 'git log --merge' - See commits that caused conflict
- 'git diff --ours' - See your changes
- 'git diff --theirs' - See their changes

## Red Flags
- Resolving same conflict repeatedly (structural problem)
- Conflicts in generated files (update .gitignore)
- Conflicts every merge (branches too long-lived)
