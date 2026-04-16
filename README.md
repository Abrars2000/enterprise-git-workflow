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
<img width="958" height="292" alt="Screenshot -2" src="https://github.com/user-attachments/assets/21a281b6-3d79-4a3d-810b-73ac27336cb3" />
<img width="908" height="935" alt="Screenshot -3" src="https://github.com/user-attachments/assets/33374667-7c9f-4fb1-a591-3e72ccab9754" />
<img width="966" height="202" alt="Screenshot -4" src="https://github.com/user-attachments/assets/36b6d0e2-f950-4fec-bbe8-4bfda716487a" />
<img width="945" height="813" alt="Screenshot -6" src="https://github.com/user-attachments/assets/727f1ffd-ec47-4652-8e64-68af6ac2e05c" />
<img width="932" height="266" alt="Screenshot -7" src="https://github.com/user-attachments/assets/cb778527-9b1b-4bc5-b849-da9a677988c3" />
<img width="946" height="906" alt="Screenshot -8" src="https://github.com/user-attachments/assets/e82a574c-4f6e-4d4d-9368-09c7130d5180" />
<img width="963" height="1056" alt="Screenshot -9" src="https://github.com/user-attachments/assets/55d11769-b796-4b8e-903d-c5072e1794fa" />
<img width="958" height="113" alt="Screenshot -10" src="https://github.com/user-attachments/assets/938b69cf-2f50-4dcc-bfd8-4cd198d0abf4" />
<img width="948" height="296" alt="Screenshot-5" src="https://github.com/user-attachments/assets/306d874c-33ac-4170-ade7-9ffd714fa9d9" />





## 🌿 Branch Structure
- main — Production ready code
- develop — Integration branch
- feature/login — Login feature
- feature/payment — Payment feature
- feature/profile — Profile feature
- bugfix/login-error — Bug fix branch
