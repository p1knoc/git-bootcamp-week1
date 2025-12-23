# .gitignore Pattern Guide

## Basic Patterns
- '*.class' - Ignore all .class files
- 'target/' - Ignore target directory
- '!important.jar' - Exception (don't ignore this)

## Real-World Examples

### Why We Ignore Each Type

#### Build Artifacts ('target/', '*.class')
- Generated during compilation
- Different on each machine
- Can be rebuilt anytime
- Bloat repository size

#### IDE Files ('.idea/', '*.iml')
- Developer-specific settings
- Cause merge conflicts
- Not needed for project to work
- Each dev has different IDE setup

#### Sensitive Files ('*.env', 'secret.*)
- NEVER commit passwords, API keys, tokens
- Security risk if leaked
- Use environment variable instead
- In workplace: instant security incident!

#### Logs ('*.log')
- Temporary runtime data
- Usually large files
- No value in version control
- Use log aggregation services instead

### Testing .gitignore

# Create a test directory
mkdir gitignore-test
cd gitignore-test

# Create files matching patterns
touch test.class
touch debug.log
mkdir target
touch target/output.jar

# Check they're ignored
git status

# No files shown = .gitignore working!
