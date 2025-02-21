To **update your local repository** with the latest changes from GitHub, follow these steps:

---

### **1. Navigate to Your Local Repository**
Open a terminal and go to the project folder:  
```sh
cd /path/to/your-repository
```

---

### **2. Check Your Current Branch**
Make sure you're on the correct branch:  
```sh
git branch
```
If needed, switch to the main branch:  
```sh
git checkout main  # or master, depending on your repository
```

---

### **3. Fetch and Pull Latest Changes**
Run the following command to update your local branch with the latest changes from GitHub:  
```sh
git pull origin main
```
(Replace `main` with `master` or any other branch you're working on.)

- **`git fetch`** downloads changes without applying them.
- **`git pull`** downloads and applies the latest changes.

---

### **4. Resolve Merge Conflicts (If Any)**
If there are conflicts, Git will ask you to resolve them.  

1. Open the conflicting files and manually fix the issues.
2. After fixing, **stage the changes**:
   ```sh
   git add .
   ```
3. Commit the resolved files:
   ```sh
   git commit -m "Resolved merge conflicts"
   ```
4. Complete the pull:
   ```sh
   git pull origin main
   ```

---

### **5. Verify the Update**
Check the latest commit log to confirm your local repo is updated:
```sh
git log --oneline -5
```
(This shows the last 5 commits.)

---

### **6. (Optional) Reset Local Changes to Match GitHub**
If you want to discard local changes and reset to GitHub’s latest version:
```sh
git reset --hard origin/main
```
**⚠️ Warning:** This will **delete all local changes** that are not committed.

---

### **Now Your Local Repo is Up to Date!** 
You can now continue working on your project.
