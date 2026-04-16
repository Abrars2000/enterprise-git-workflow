# enterprise-git-workflow
# 🚀 Enterprise Git Workflow Assignment

## 📋 All Commands Used

### Repository Setup
git clone <repo-url>
git checkout -b develop
git checkout -b feature/login

### Branching
git checkout -b feature/payment
git checkout -b feature/profile
git checkout -b bugfix/login-error

### Merge Strategy
git checkout develop
git merge feature/payment --no-ff -m "merge: integrate payment feature"

### Rebase Strategy
git checkout feature/profile
git rebase develop
git push origin feature/profile --force

### Interactive Rebase
git rebase -i HEAD~5

---

## 🔀 Merge vs Rebase

| Feature | Merge | Rebase |
|---------|-------|--------|
| History | সব commit সংরক্ষণ করে | Linear history তৈরি করে |
| Extra Commit | Merge commit তৈরি হয় | কোনো extra commit নেই |
| Use Case | Team collaboration | Clean feature branch |
| Safety | নিরাপদ | History rewrite করে |

**Merge:** দুটো branch একসাথে জুড়ে দেয়, একটি merge commit তৈরি হয়।
**Rebase:** Commits গুলো base branch এর উপরে নতুনভাবে apply করে, পরিষ্কার history তৈরি করে।

---

## 🗜️ Squash & Reword

**Squash:** একাধিক ছোট commit কে একটি বড় commit এ পরিণত করে।
**Reword:** পুরানো commit এর message পরিবর্তন করে।

---

## 📸 Screenshots
<img width="1632" height="785" alt="Screenshot -1" src="https://github.com/user-attachments/assets/547d8a64-9ed2-4e46-bef3-893175c39d6b" />



## 🌿 Branch Structure
- main — Production ready code
- develop — Integration branch
- feature/login — Login feature
- feature/payment — Payment feature
- feature/profile — Profile feature
- bugfix/login-error — Bug fix branch
