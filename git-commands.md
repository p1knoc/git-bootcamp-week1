# Git Commands Quick Reference

## Daily Workflow
git status		# Check what's changed
git add <file>		# Stage specific file
git add .		# Stage all changes
git commit -m "msg"	# Commit staged changes
git push origin main	# Push to GitHub

## Branching
git branch		# List branches
git branch <name>	# Create branch
git checkout -b <name>	# Create and switch
git checkout <name>	# Switch branches
git merge <name>	# Merge branch into current
git branch -d <name>	# Delete merged branch

## Viewing History
git log			# Full history
git log --oneline	# Condensed view
git log --graph --all	# Visual branch history
git diff		# Unstaged changes
git diff --staged	# Staged changes
