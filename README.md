# 📦 Copy Repository from Another GitHub Account

This guide explains how to copy a repository from another GitHub account to your own account.

---

## 🚀 Steps

### 1. Clone the repository (from another account)

```bash
git clone https://github.com/OTHER_USERNAME/REPO_NAME.git
cd REPO_NAME
```

---

### 2. Check current remote

```bash
git remote -v
```

This shows the current repository connection (origin).

---

### 3. Remove old remote

```bash
git remote remove origin
```

---

### 4. Add your GitHub repository as new remote

```bash
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git
```

---

### 5. Push code to your repository

```bash
git push -u origin main
```

If your branch is `master`, use:

```bash
git push -u origin master
```

---

## ⚠️ Common Issues

### Permission denied

* Make sure you are logged into the correct GitHub account.

### Rejected push

```bash
git push -u origin main --force
```

---

## ✅ Result

* Repository is successfully copied to your GitHub account
* All files and commit history are preserved

---

## 💡 Alternative (Quick Method)

```bash
git push https://github.com/YOUR_USERNAME/REPO_NAME.git
```

---

## 📌 Notes

* Replace `YOUR_USERNAME` with your GitHub username
* Replace `REPO_NAME` with your repository name
* Replace `OTHER_USERNAME` with the source repository owner

---
