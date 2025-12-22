# Day 4 Learning Notes

## Merge Conflicts

### What I Learned
Conflicts aren't errors - they're Git saying "I need human judgement here."

### Key Skills
- Reading conflict markers
- Resolving conflicts manually
- Staging resolved files
- Completing conflict merges
- Using git status during conflicts

### Conflict Resolution Process
1. 'git merge <branch>' triggers conflict
2. 'git status' shows conflicted files
3. Open files, look for '<<<<<<<', '========', '>>>>>>>>'
4. Edit files to resolve
5. 'git add <resolved-files>'
6. 'git commit' to complete merge

### Real-World Insights
- Small, frequent merges = fewer conflicts
- Communication prevents most conflicts
- Testing after resolution is crucial
- Good merge messages help future developers

### Linux Integration
- Used 'cat' to view conflict markers
- Used 'grep' to search for conflicts: 'grep -r "<<<<<<<" .'
- Used pipes to count conflicts: 'git diff --check | wc -l'

### Confidence Boost
I can now handle the conflicts that intimidated me before. This is a crucial team development skill.
