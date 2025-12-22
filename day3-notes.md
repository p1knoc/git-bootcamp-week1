# Day 3 Learning Notes

## Branching Concepts

### Key Terms
- **Branch**: A pointer to a commit (think: parallel universe)
- **HEAD**: Pointer to current branch
- **Checkout**: Switch between branches
- **Merge**: Combine branch changes

### Commands Mastered
- 'git branch' - List branches
- 'git checkout -b <name>' - Create and switch to branch
- 'git checkout <name>' - Switch to existing branch
- 'git merge <branch>' - Merge branch into current branch
- 'git branch -d <name>' - Delete merged branch

## Real-World Application
Branches let teams work on features simultaneously without stepping on each other's toes. Before merging to main, code goes through review and testing.

## Linux Integration
- Branch names can't have spaces (use kebab-case or snake_case)
- Use tab completion for branch names
- 'git branch' output can be piped to other commands
