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
- Merge conflicts? → Start with Repository 2
- Cleaning up messy history? → Start with Repository 3
- Understanding push/pull? → Start with Repository 5
- Recovering from mistakes? → Start with Repository 6
- New to Git? → Start with Repository 1

**"What's my experience level?"
- 🟢 Beginner: Repos 1, 7, 2, 5
- 🟡 Intermediate: Repos 2, 5, 3, 4, 8
- 🔴 Advanced: Repos 3, 4, 6, 9

### Step 3: Clone All Repositories

**Recommended**: Clone all repositories into a common parent folder:

```bash
# Create a dedicated folder for all Git Mastery repos
mkdir ~/git-mastery
cd ~/git-mastery

# Clone all repositories
git clone https://github.com/TheCodeGarage/git-mastery-00-hub
git clone https://github.com/TheCodeGarage/git-mastery-01-foundations
git clone https://github.com/TheCodeGarage/git-mastery-02-merge-conflicts
git clone https://github.com/TheCodeGarage/git-mastery-03-rebasing
git clone https://github.com/TheCodeGarage/git-mastery-04-history-rewriting
git clone https://github.com/TheCodeGarage/git-mastery-05-remote-workflows
git clone https://github.com/TheCodeGarage/git-mastery-06-recovery-operations
git clone https://github.com/TheCodeGarage/git-mastery-07-branching-strategies
git clone https://github.com/TheCodeGarage/git-mastery-08-stash-cherry-pick
git clone https://github.com/TheCodeGarage/git-mastery-09-debugging-bisect
git clone https://github.com/TheCodeGarage/git-mastery-quiz
```

**Why this structure?**
- Navigate easily between repos using `cd ../`
- Quiz game references work correctly
- All repos stay independent (can reset one without affecting others)

### Step 4: Optional - Create Practice Copies

**Want to experiment safely?** Work in copies:

```bash
# Create practice workspace
mkdir ~/git-practice
cd ~/git-practice

# Copy a repo you want to experiment with
cp -r ~/git-mastery/git-mastery-02-merge-conflicts .
cd git-mastery-02-merge-conflicts
```

**Important**: Work in a COPY if you want to experiment freely. The original stays clean for reference!

## Understanding the Structure

### Recommended Folder Structure

Clone all repositories into a common parent folder:

```
git-mastery/                           # Your parent folder
├── git-mastery-00-hub/               # This hub - main navigation
├── git-mastery-quiz/                 # Interactive quiz application
├── git-mastery-01-foundations/       # Git basics practice
├── git-mastery-02-merge-conflicts/   # Merge conflict practice
├── git-mastery-03-rebasing/          # Rebasing practice
├── git-mastery-04-history-rewriting/ # History editing practice
├── git-mastery-05-remote-workflows/  # Remote operations practice
├── git-mastery-06-recovery-operations/ # Recovery practice
├── git-mastery-07-branching-strategies/ # Branching practice
├── git-mastery-08-stash-cherry-pick/ # Stash & cherry-pick practice
└── git-mastery-09-debugging-bisect/  # Debugging practice
```

**All repositories are independent** - each is its own GitHub repo with complete Git history!

### Inside Each Practice Repository

```
git-mastery-02-merge-conflicts/
├── .git/                       # Git repository data
├── README.md                   # Topic overview & objectives
├── EXERCISES.md                # Hands-on practice exercises
├── GIT-CHEATSHEET.md          # Quick command reference
├── SOLUTIONS.md                # Exercise solutions (try first!)
├── TROUBLESHOOTING.md          # Common issues & fixes
└── [source files]              # Code with 40-50 commits
```

## Your First Practice Session

### 1. Navigate to a Repository

Let's start with **Merge Conflicts** as an example:

```bash
cd ~/git-mastery/git-mastery-02-merge-conflicts
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
cd ../git-mastery-quiz
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

**Option 2: Re-Clone Repository**
```bash
# Delete the repository
cd ~/git-mastery
rm -rf git-mastery-02-merge-conflicts

# Clone fresh from GitHub
git clone https://github.com/TheCodeGarage/git-mastery-02-merge-conflicts
cd git-mastery-02-merge-conflicts
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
# Delete all repositories
rm -rf ~/git-mastery

# Start fresh - clone again from GitHub
mkdir ~/git-mastery
cd ~/git-mastery
# Clone repositories you need
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
# Should end with: /git-mastery-XX-topic-name/

# Navigate to repository
cd ~/git-mastery/git-mastery-02-merge-conflicts
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
Start here: [Foundations](../git-mastery-01-foundations/README.md) or [Branching Strategies](../git-mastery-07-branching-strategies/README.md)

### 🟡 Intermediate
Start here: [Merge Conflicts](../git-mastery-02-merge-conflicts/README.md) or [Remote Workflows](../git-mastery-05-remote-workflows/README.md)

### 🔴 Advanced
Start here: [Rebasing](../git-mastery-03-rebasing/README.md), [History Rewriting](../git-mastery-04-history-rewriting/README.md), or [Recovery Operations](../git-mastery-06-recovery-operations/README.md)

---

## All Practice Repositories

| Repository | Difficulty | Focus Area | Estimated Time |
|-----------|-----------|-----------|----------------|
| [01 - Foundations](../git-mastery-01-foundations/README.md) | 🟢 Beginner | Basic Git commands, commits, branches | 2-3 hours |
| [02 - Merge Conflicts](../git-mastery-02-merge-conflicts/README.md) | 🟡 Intermediate | Resolving merge conflicts | 4-5 hours |
| [03 - Rebasing](../git-mastery-03-rebasing/README.md) | 🔴 Advanced | Rebase operations, interactive rebase | 5-6 hours |
| [04 - History Rewriting](../git-mastery-04-history-rewriting/README.md) | 🔴 Advanced | Amend, reset, revert, filter-branch | 6-7 hours |
| [05 - Remote Workflows](../git-mastery-05-remote-workflows/README.md) | 🟡 Intermediate | Push, pull, fetch, remote branches | 4-5 hours |
| [06 - Recovery Operations](../git-mastery-06-recovery-operations/README.md) | 🔴 Advanced | Reflog, fsck, data recovery | 6-8 hours |
| [07 - Branching Strategies](../git-mastery-07-branching-strategies/README.md) | 🟢 Beginner | Feature branches, Git Flow, workflows | 3-4 hours |
| [08 - Stash & Cherry-Pick](../git-mastery-08-stash-cherry-pick/README.md) | 🟡 Intermediate | Stashing changes, cherry-picking commits | 4-5 hours |
| [09 - Debugging & Bisect](../git-mastery-09-debugging-bisect/README.md) | 🔴 Advanced | Git blame, bisect, debugging | 5-6 hours |
| [Quiz Game](../git-mastery-quiz/README.md) | All Levels | Test your knowledge interactively | 30 min per topic |

### 🎯 Targeted Practice
Jump to: [Choose from Main README](README.md#-practice-repositories)

---

**Questions?** Check the TROUBLESHOOTING.md in each practice repository or refer to the Git documentation.

**Happy Learning!** 🚀
