Here is the **Markdown-formatted** short and informative version for your GitHub README notes:

```markdown
# 🔄 Git Commands: Revert to a Previous Version

## ✅ Reset to a Previous Commit (Deletes Changes)
```bash
git log --oneline  # Find commit hash
git reset --hard <commit-hash>  # Go back to that commit
git push --force  # Update remote (⚠️ Overwrites history)
```
🚨 **Warning:** Use `--force` only if you're sure. It rewrites history.

---

## ✅ Revert the Last Commit (Safe for Shared Repos)
```bash
git revert HEAD  # Creates a new commit that undoes the last one
git push
```
✅ **Best for undoing commits without history rewrite.**

---

## ✅ Checkout an Old Version Without Changing History
```bash
git checkout <commit-hash>  # View an old version
```
To create a new branch from that version:
```bash
git checkout -b old-version <commit-hash>
```

---

## ✅ View Commit History in GitHub UI
1. Go to **GitHub Repo** → Click **Commits**.
2. Find the commit → Copy its **hash**.
3. Use `git checkout <commit-hash>` or `git revert HEAD`.

---

💡 **Use the right method depending on whether you need to erase, revert, or just check an old version.**
```

This will format correctly when pasted into **GitHub README** or any Markdown file. 📜🚀  
Let me know if you need any modifications! 😊
