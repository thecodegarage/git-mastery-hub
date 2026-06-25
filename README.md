# Git Mastery & Practice 🚀

**The Complete Git Learning System for All Experience Levels**

Master Git by practicing in real repositories designed around the topics developers struggle with most.

## 🎯 What Makes This Different?

- **9 Independent Practice Repositories** - Each focused on a specific topic
- **40-50 Commits Per Repo** - Realistic, messy scenarios ready for you to practice
- **Jump to Any Topic** - Start exactly where you need help
- **200+ Question Quiz Game** - Test your knowledge and track progress
- **Safe Experimentation** - Mess up? Just re-clone and start fresh!

## 📚 Practice Repositories

Each repository is **completely independent** on GitHub. Clone only what you need, reset without losing progress in other repos!

### 🟢 Foundation (Start Here if New to Git)

| # | Topic | Repository | Difficulty |
|---|-------|------------|------------|
| 0 | **Git Basics & Daily Workflow** | [`git-practice-foundations`](https://github.com/TheCodeGarage/git-practice-foundations) | 🟢 Beginner |

```bash
git clone https://github.com/TheCodeGarage/git-practice-foundations
```

**Learn:** Setup, init, clone, add, commit, push, pull, basic branching, viewing history

---

### 🔴 Top Priority (Most Common Struggle Areas)

| # | Topic | Repository | Difficulty |
|---|-------|------------|------------|
| 1 | **Merge Conflicts** | [`git-practice-merge-conflicts`](https://github.com/TheCodeGarage/git-practice-merge-conflicts) | 🟡 Intermediate |
| 2 | **Rebasing** | [`git-practice-rebasing`](https://github.com/TheCodeGarage/git-practice-rebasing) | 🔴 Advanced |
| 3 | **History Rewriting** | [`git-practice-history-rewriting`](https://github.com/TheCodeGarage/git-practice-history-rewriting) | 🔴 Advanced |
| 4 | **Remote Workflows** | [`git-practice-remote-workflows`](https://github.com/TheCodeGarage/git-practice-remote-workflows) | 🟡 Intermediate |
| 5 | **Recovery Operations** | [`git-practice-recovery-operations`](https://github.com/TheCodeGarage/git-practice-recovery-operations) | 🔴 Advanced |

```bash
# Clone specific topics you struggle with
git clone https://github.com/TheCodeGarage/git-practice-merge-conflicts
git clone https://github.com/TheCodeGarage/git-practice-rebasing
# etc...
```

---

### 🟡 Secondary Important Areas

| # | Topic | Repository | Difficulty |
|---|-------|------------|------------|
| 6 | **Branching Strategies** | [`git-practice-branching-strategies`](https://github.com/TheCodeGarage/git-practice-branching-strategies) | 🟢 Beginner |
| 7 | **Stash & Cherry-Pick** | [`git-practice-stash-cherry-pick`](https://github.com/TheCodeGarage/git-practice-stash-cherry-pick) | 🟡 Intermediate |
| 8 | **Debugging & Bisect** | [`git-practice-debugging-bisect`](https://github.com/TheCodeGarage/git-practice-debugging-bisect) | 🔴 Advanced |

```bash
git clone https://github.com/TheCodeGarage/git-practice-branching-strategies
git clone https://github.com/TheCodeGarage/git-practice-stash-cherry-pick
git clone https://github.com/TheCodeGarage/git-practice-debugging-bisect
```

---

## 🎮 Interactive Quiz Game

Test your Git knowledge with our interactive React quiz featuring 200+ questions!

**Repository:** [`git-mastery-quiz`](https://github.com/TheCodeGarage/git-mastery-quiz)

```bash
git clone https://github.com/TheCodeGarage/git-mastery-quiz
cd git-mastery-quiz
npm install
npm run dev
```

**Features:**
- ✅ 200+ questions covering all topics
- ✅ Filter by specific topic or take comprehensive test
- ✅ Instant feedback with detailed explanations
- ✅ Track your progress and scores
- ✅ Difficulty levels: Beginner → Expert
- ✅ Challenge mode with random questions
- ✅ Dark mode support

---

## 🚀 Getting Started

### Prerequisites
- **Git** installed - [Download here](https://git-scm.com/downloads)
- **Basic command line** knowledge
- **Text editor** - VS Code recommended
- **Node.js** (for quiz game only) - [Download](https://nodejs.org/)

### Quick Start Guide

#### 1. Choose Your Starting Point

**New to Git?**
```bash
git clone https://github.com/TheCodeGarage/git-practice-foundations
cd git-practice-foundations
```

**Struggle with specific topic?**
```bash
# Merge conflicts
git clone https://github.com/TheCodeGarage/git-practice-merge-conflicts

# Rebasing
git clone https://github.com/TheCodeGarage/git-practice-rebasing

# etc...
```

#### 2. Work Through Exercises

Each repository contains:
- **README.md** - Topic overview & objectives
- **EXERCISES.md** - Hands-on practice (12+ exercises)
- **GIT-CHEATSHEET.md** - Command reference
- **SOLUTIONS.md** - Detailed solutions
- **TROUBLESHOOTING.md** - Common issues & fixes

#### 3. Test Your Knowledge

After completing exercises, take the quiz for that topic:
```bash
git clone https://github.com/TheCodeGarage/git-mastery-quiz
cd git-mastery-quiz
npm install && npm run dev
```

Aim for **80%+ score** before moving to next topic!

#### 4. Reset & Retry

Messed up? Just re-clone that specific repo:
```bash
# Delete your working copy
rm -rf git-practice-merge-conflicts

# Clone fresh
git clone https://github.com/TheCodeGarage/git-practice-merge-conflicts

# Your other repos remain untouched! ✅
```

---

## 📖 Learning Paths

### 🟢 Complete Beginner (Never Used Git)
**Duration:** 3-5 weeks

1. **Git Basics & Daily Workflow** (Foundation)
2. **Branching Strategies** 
3. **Stash & Cherry-Pick**
4. **Merge Conflicts**
5. **Remote Workflows**

### 🟡 Intermediate (Know Basics, Want to Level Up)
**Duration:** 4-6 weeks

1. **Git Basics & Daily Workflow** (Quick review)
2. **Merge Conflicts**
3. **Remote Workflows**
4. **Rebasing**
5. **History Rewriting**
6. **Stash & Cherry-Pick**

### 🔴 Advanced (Master Everything)
**Duration:** 6-8 weeks

Complete all 9 repositories in order:
1. Foundations → Branching → Stash/Cherry-Pick → Merge Conflicts → Remote Workflows → Rebasing → History Rewriting → Recovery → Debugging/Bisect

---

## 💡 Why Independent Repositories?

### Key Benefits:
✅ **Clone only what you need** - Smaller, faster downloads
✅ **Reset individual topics** - Don't lose progress in other repos
✅ **Work on multiple topics** - Switch between repos freely
✅ **Fork to save progress** - Keep your work on GitHub
✅ **Update independently** - Get latest exercises for specific topics

### Example Workflow:
```bash
# You're working on multiple topics
~/practice/
├── git-practice-foundations/       ✅ Completed
├── git-practice-merge-conflicts/   🔄 In progress (exercise 8/12)
└── git-practice-rebasing/          🔄 In progress (exercise 5/15)

# Messed up rebasing? Re-clone just that one:
rm -rf git-practice-rebasing
git clone https://github.com/TheCodeGarage/git-practice-rebasing

# Your merge-conflicts progress is safe! ✅
```

---

## 📊 Progress Tracking

Track your journey through all 9 repositories:

- [ ] 0. **Git Basics & Daily Workflow** - Quiz Score: ____%
- [ ] 1. **Merge Conflicts** - Quiz Score: ____%
- [ ] 2. **Rebasing** - Quiz Score: ____%
- [ ] 3. **History Rewriting** - Quiz Score: ____%
- [ ] 4. **Remote Workflows** - Quiz Score: ____%
- [ ] 5. **Recovery Operations** - Quiz Score: ____%
- [ ] 6. **Branching Strategies** - Quiz Score: ____%
- [ ] 7. **Stash & Cherry-Pick** - Quiz Score: ____%
- [ ] 8. **Debugging & Bisect** - Quiz Score: ____%

---

## 🎓 Learning Philosophy

This system is built on research-backed principles:

1. **Practice in Context** - Real repositories with real scenarios
2. **Fail Safely** - Experiment without fear of breaking things
3. **Learn by Doing** - Hands-on practice beats passive reading
4. **Measure Progress** - Quizzes validate understanding
5. **Start Anywhere** - No forced linear progression
6. **Independent Practice** - Each topic is self-contained

## 🤝 Contributing

Found an issue? Have suggestions? Want to add exercises?

Each repository has its own CONTRIBUTING.md with guidelines for that topic.

For general questions or suggestions about the learning system:
- Open an issue in the [`git-mastery-hub`](https://github.com/TheCodeGarage/git-mastery-hub) repository
- Reach out via [TheCodeGarage.com](https://thecodegarage.com)

## 📝 License

All repositories are MIT Licensed - Use freely for learning and teaching!

## 🌟 Acknowledgments

Built with ❤️ by [The Code Garage](https://thecodegarage.com) for developers who want to truly master Git.

Based on empirical data about what developers struggle with most, combined with proven learning techniques.

---

## 🚀 Ready to Start?

### For Complete Beginners:
```bash
git clone https://github.com/TheCodeGarage/git-practice-foundations
cd git-practice-foundations
cat README.md  # Start here!
```

### For Experienced Developers:
Pick your weak spot and dive in! Each repo is independent.

### Questions?
See [GETTING-STARTED.md](GETTING-STARTED.md) for comprehensive setup and usage guide.

---

**Happy Learning!** 🎯 Master Git one topic at a time.
4. **Measure Progress** - Quiz validates understanding
5. **Start Anywhere** - No forced sequences

## 📝 License

MIT License - Use freely for learning!

## 🌟 Acknowledgments

Built with ❤️ for developers who want to truly master Git, based on empirical data about what developers struggle with most.

---

**Ready to master Git?** Start with [Getting Started](GETTING-STARTED.md) or jump into a [practice repository](practice-repos/)!
