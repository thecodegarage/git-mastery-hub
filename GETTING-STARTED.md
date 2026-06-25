# Getting Started with Git Mastery & Practice

Complete guide to using this learning system effectively.

## 📋 Table of Contents

1. [System Requirements](#system-requirements)
2. [Initial Setup](#initial-setup)
3. [Understanding the Structure](#understanding-the-structure)
4. [Your First Practice Session](#your-first-practice-session)
5. [Best Practices](#best-practices)
6. [Troubleshooting](#troubleshooting)

## System Requirements

### Required
- **Git**: Version 2.30 or higher
  ```bash
  git --version
  ```
  If not installed: [Download Git](https://git-scm.com/downloads)

- **Terminal/Command Line**: 
  - Windows: Git Bash, PowerShell, or WSL
  - Mac: Terminal or iTerm2
  - Linux: Any terminal

- **Text Editor**: 
  - VS Code (recommended) - [Download](https://code.visualstudio.com/)
  - Sublime Text, Atom, or any editor

### Optional (for Quiz Game)
- **Node.js**: Version 18+ - [Download](https://nodejs.org/)
- **npm**: Comes with Node.js

## Initial Setup

### Step 1: Verify Git Installation

```bash
# Check Git is installed
git --version

# Configure your identity (if not already done)
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

# Optional: Set default editor
git config --global core.editor "code --wait"
```

### Step 2: Choose Your Starting Point

Ask yourself:

**"What do I struggle with most?"**
- Merge conflicts? → Start with Repository 1
- Cleaning up messy history? → Start with Repository 2
- Understanding push/pull? → Start with Repository 4
- Recovering from mistakes? → Start with Repository 5
- New to Git? → Start with Repository 6

**"What's my experience level?"**
- 🟢 Beginner: Repos 6, 7, 1, 4
- 🟡 Intermediate: Repos 1, 4, 2, 3, 7
- 🔴 Advanced: Repos 2, 3, 5, 8

### Step 3: Set Up Your Practice Environment

Create a dedicated workspace:

```bash
# Create practice workspace
mkdir ~/git-practice
cd ~/git-practice

# Copy the practice repo you want to work with
# Example: Merge Conflicts
cp -r /path/to/git-mastery-and-practice/practice-repos/01-merge-conflicts .
cd 01-merge-conflicts
```

**Important**: Work in a COPY, not the original! This way you can always reset.

## Understanding the Structure

### Main Folder Structure

```
git-mastery-and-practice/
├── README.md                    # You are here - main navigation
├── GETTING-STARTED.md          # This file - detailed guide
├── quiz-game/                  # Interactive quiz application
└── practice-repos/             # 8 independent repositories
    ├── 01-merge-conflicts/
    ├── 02-rebasing/
    ├── 03-history-rewriting/
    ├── 04-remote-workflows/
    ├── 05-recovery-operations/
    ├── 06-branching-strategies/
    ├── 07-stash-cherry-pick/
    └── 08-debugging-bisect/
```

### Inside Each Practice Repository

```
01-merge-conflicts/
├── .git/                       # Git repository data
├── README.md                   # Topic overview & objectives
├── EXERCISES.md                # Hands-on practice exercises
├── GIT-CHEATSHEET.md          # Quick command reference
├── SOLUTIONS.md                # Exercise solutions (try first!)
├── TROUBLESHOOTING.md          # Common issues & fixes
└── [source files]              # Code with 40-50 commits
```

## Your First Practice Session

### 1. Pick a Repository

Let's start with **Merge Conflicts** as an example:

```bash
cd practice-repos/01-merge-conflicts
```

### 2. Read the README

```bash
# Open in your editor
code README.md

# Or view in terminal
cat README.md | less
```

The README tells you:
- What you'll learn
- Prerequisites (what you should know first)
- Learning objectives
- How the repository is set up

### 3. Explore the Commit History

```bash
# View all commits with graph
git log --all --graph --oneline --decorate

# View last 20 commits
git log --oneline -n 20

# View commits by author
git log --author="Sarah"
```

This repository has 40-50 commits from multiple "team members" - just like a real project!

### 4. Start Exercise 1

```bash
# Open exercises file
code EXERCISES.md
```

Each exercise has:
- **Objective**: What you'll learn
- **Scenario**: The problem to solve
- **Tasks**: Step-by-step instructions
- **Validation**: How to check if you succeeded
- **Learning Points**: Key takeaways

### 5. Complete the Exercise

Follow the instructions, try the commands, make mistakes! 

**Tips:**
- Read the full exercise before starting
- Try commands yourself before looking at solutions
- Use `git status` frequently
- Don't worry about breaking things!

### 6. Check the Solution

Only after attempting:

```bash
code SOLUTIONS.md
```

Compare your approach with the provided solution.

### 7. Take the Quiz

After completing all exercises in a repository:

```bash
cd ../../quiz-game
npm install    # First time only
npm run dev
```

- Select the topic you just completed
- Aim for 80%+ score
- Review any questions you missed

## Best Practices

### Do's ✅

- **Read before doing** - Skim the entire exercise first
- **Experiment freely** - Try different approaches
- **Use git status** - Check state frequently
- **Read Git's output** - It often tells you what to do next
- **Make mistakes** - That's how you learn!
- **Reset and retry** - Practice the same exercise multiple times
- **Take breaks** - Let concepts sink in
- **Keep a notes file** - Document what you learn

### Don'ts ❌

- **Don't rush** - Take time to understand each concept
- **Don't skip validation** - Always verify your work
- **Don't peek at solutions** - Try first, struggle a bit
- **Don't work when tired** - Git requires focus
- **Don't mix topics** - Complete one before starting another
- **Don't fear breaking things** - You can always re-clone!

## Learning Workflow

### Recommended Pattern

```
1. Read README (5 minutes)
   ↓
2. Explore commits (5 minutes)
   ↓
3. Complete Exercise 1 (15-30 minutes)
   ↓
4. Check solution (5 minutes)
   ↓
5. Repeat for remaining exercises
   ↓
6. Take quiz (15 minutes)
   ↓
7. Review incorrect answers (10 minutes)
   ↓
8. Move to next topic or retake quiz
```

### Time Estimates

Per Repository:
- 🟢 Beginner topics: 2-4 hours
- 🟡 Intermediate topics: 4-6 hours
- 🔴 Advanced topics: 6-8 hours

Complete System:
- 🟢 Beginner path: 15-25 hours (2-4 weeks)
- 🟡 Intermediate path: 25-35 hours (4-6 weeks)
- 🔴 Advanced path: 35-50 hours (6-8 weeks)

## Resetting & Starting Over

### Messed Up a Repository?

**Option 1: Reset to Clean State**
```bash
# View what you changed
git status

# Discard all changes (careful!)
git reset --hard HEAD
git clean -fd

# Now back to original state
```

**Option 2: Re-Copy Original**
```bash
# Delete your working copy
cd ~/git-practice
rm -rf 01-merge-conflicts

# Copy fresh from original
cp -r /path/to/git-mastery-and-practice/practice-repos/01-merge-conflicts .
cd 01-merge-conflicts
```

**Option 3: Use Git to Reset**
```bash
# Find the original commit
git log --all --oneline

# Reset to it
git reset --hard <original-commit>
```

### Completely Start Over?

```bash
# Delete all your practice work
rm -rf ~/git-practice

# Start fresh
mkdir ~/git-practice
# Copy repositories again
```

## Troubleshooting

### Git Commands Not Working?

```bash
# Verify Git is in PATH
git --version

# Verify you're in a Git repository
git status
# Should NOT show: "fatal: not a git repository"

# Check current directory
pwd
```

### Can't Find Exercise Files?

```bash
# List all files (including hidden)
ls -la

# Verify you're in the right directory
pwd
# Should end with: /practice-repos/XX-topic-name/

# Navigate correctly
cd /path/to/git-mastery-and-practice/practice-repos/01-merge-conflicts
```

### Merge Conflicts Stuck?

```bash
# See what's in conflict
git status

# Abort the merge and start over
git merge --abort

# Or abort rebase
git rebase --abort
```

### Lost Where You Are?

```bash
# See current branch and status
git status

# See all branches
git branch -a

# See recent activity
git reflog --all

# View commit graph
git log --all --graph --oneline -n 20
```

### Commands Don't Match Your Git Version?

Some commands differ by version. If a command doesn't work:

```bash
# Check version
git --version

# Look for alternative in cheatsheet
cat GIT-CHEATSHEET.md | grep "alternative"
```

## Getting Help

### Within Each Repository

1. **TROUBLESHOOTING.md** - Common issues for that topic
2. **GIT-CHEATSHEET.md** - Command reference
3. **SOLUTIONS.md** - See how it should be done

### Git's Built-in Help

```bash
# Help for any command
git help <command>
git <command> --help

# Example
git help merge
git rebase --help

# Quick summary
git <command> -h
```

### External Resources

- [Git Documentation](https://git-scm.com/doc)
- [Pro Git Book](https://git-scm.com/book) (free online)
- GitHub Community Forums
- Stack Overflow (search: "git [your issue]")

## Next Steps

Ready to start? Pick your path:

### 🟢 Beginner
Start here: [Branching Strategies](practice-repos/06-branching-strategies/README.md)

### 🟡 Intermediate
Start here: [Merge Conflicts](practice-repos/01-merge-conflicts/README.md)

### 🔴 Advanced
Start here: [Rebasing](practice-repos/02-rebasing/README.md)

### 🎯 Targeted Practice
Jump to: [Choose from Main README](README.md#practice-repositories)

---

**Questions?** Check the TROUBLESHOOTING.md in each practice repository or refer to the Git documentation.

**Happy Learning!** 🚀
