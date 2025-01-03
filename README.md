# Hotwax_Git_Part3

### **Part 1: Git Commit Basics**
**Task**: Stage and commit files, then view commit history.  
**Solution**:
1. Open the terminal and navigate to your project directory:  
   
   cd your-project-directory
   
2. Stage files:  
   
   git add .
   
3. Commit changes:  
   
   git commit -m "Initial commit"
   
4. View commit history:  
   
   git log

### **Part 2: Reverting a Commit**
**Task**: Revert a commit.  
**Solution**:
1. Check commit history and copy the commit ID:  
   
   git log
   
2. Revert the commit:  
   
   git revert <commit-id>

### **Part 3: Merge Conflicts**
**Task**: Create and resolve merge conflicts.  
**Solution**:
1. Create and switch to a new branch:  

  - git branch new-branch
  - git checkout new-branch
   
2. Make changes and commit.  
3. Switch back to the `main` branch:  
   
   git checkout main
   
4. Merge the new branch into `main`:  
   
   git merge new-branch
   
5. If a conflict occurs, resolve it by editing the files, then complete the merge:  
   
   git add .
   git commit


### **Part 4: Cherry-Picking Commits**
**Task**: Apply specific commits from one branch to another.  
**Solution**:
1. Get the commit ID:  

   git log
   
2. Switch to the target branch and apply the commit:  
   
   git checkout target-branch
   git cherry-pick <commit-id>


### **Part 5: Fetching Branches**
**Task**: Fetch branches from a remote repository.  
**Solution**:
1. Fetch branches:  
   
   git fetch origin
   
2. Inspect the branch contents:  
   
   git checkout branch-name

### **Part 6: Syncing Forked Branch**
**Task**: Sync a forked repository with the upstream repository.  
**Solution**:
1. Add the upstream repository:
   
   git remote add upstream <original-repo-url>
   
3. Fetch changes from upstream:  
   
   git fetch upstream
   
4. Merge changes:  
   
   git merge upstream/main

### **Part 7: Merging via Command Line**
**Task**: Merge branches using the command line.  
**Solution**:
1. Create a new branch:  
   
   git branch feature-branch
   git checkout feature-branch
   
2. Make changes and commit.  
3. Merge the feature branch into `main`:  
   
   git checkout main
   git merge feature-branch
  
### **Part 8: Git Stash**
**Task**: Stash changes, switch branches, and apply the stash.  
**Solution**:
1. Stash changes:  

   git stash
   
2. Switch branches:
   
     git checkout other-branch

4. Apply the stashed changes:  

   git stash apply


### **Part 9: Pushing to Remote**
**Task**: Push changes to a remote repository.  
**Solution**:
1. Commit and push changes:  

   git commit -m "Message"
   git push origin main

### **Part 10: Rebasing Branches**
**Task**: Rebase one branch on top of another.  
**Solution**:
1. Perform the rebase:
   
   git checkout feature-branch
   git rebase main

### **Part 11: Resetting Changes**
**Task**: Understand hard and soft resets.  
**Solution**:
1. Soft reset:  
     git reset --soft <commit-id>
2. Hard reset:
     git reset --hard <commit-id>
   

### **Part 12: Creating an Issue and Fixing It**
**Task**: Create and fix an issue on GitHub.  
**Solution**:
1. Create an issue on GitHub.  
2. Fix the issue in a new branch.  
3. Submit a pull request to merge the fix.
