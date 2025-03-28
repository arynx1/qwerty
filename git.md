Great to hear that the Windows setup is working! Below is a list of common **PowerShell commands** that you might find useful when working with **Git** and **SSH** (especially for GitHub) on **Windows**.

### **Common PowerShell Commands for Git**

1. **Check Git Version**:
   To verify if Git is installed:
   ```powershell
   git --version
   ```

2. **Configure Git User (Global)**:
   Set your name and email for Git:
   ```powershell
   git config --global user.name "Your Name"
   git config --global user.email "your_email@example.com"
   ```

3. **Check Git Configuration**:
   Display the global Git configuration:
   ```powershell
   git config --list
   ```

4. **Clone a Repository**:
   Clone a GitHub repository to your local machine:
   ```powershell
   git clone git@github.com:username/repository.git
   ```

5. **Check Remote URL**:
   To view the remote URL of your repository:
   ```powershell
   git remote -v
   ```

6. **Change Remote URL**:
   If you need to switch from HTTPS to SSH for the remote URL:
   ```powershell
   git remote set-url origin git@github.com:username/repository.git
   ```

7. **Check Status**:
   See the status of your repository (changes, staging area, etc.):
   ```powershell
   git status
   ```

8. **Add Files to Staging**:
   Stage all changes:
   ```powershell
   git add .
   ```
   Stage a specific file:
   ```powershell
   git add filename.txt
   ```

9. **Commit Changes**:
   Commit your staged changes with a message:
   ```powershell
   git commit -m "Your commit message"
   ```

10. **Push Changes**:
    Push your changes to the remote repository:
    ```powershell
    git push origin main
    ```

11. **Pull Changes**:
    Pull the latest changes from the remote repository:
    ```powershell
    git pull origin main
    ```

12. **Show Commit History**:
    View the commit history for the current branch:
    ```powershell
    git log
    ```

13. **Create a New Branch**:
    Create and switch to a new branch:
    ```powershell
    git checkout -b new-branch-name
    ```

14. **Switch Branches**:
    Switch to an existing branch:
    ```powershell
    git checkout branch-name
    ```

15. **Merge a Branch**:
    Merge another branch (e.g., `feature-branch`) into your current branch:
    ```powershell
    git merge feature-branch
    ```

16. **Delete a Branch**:
    Delete a local branch:
    ```powershell
    git branch -d branch-name
    ```

17. **Stash Changes**:
    Temporarily save your uncommitted changes:
    ```powershell
    git stash
    ```
    To apply the changes later:
    ```powershell
    git stash apply
    ```

18. **Check Git SSH Connection**:
    To test if your SSH key is set up properly with GitHub:
    ```powershell
    ssh -T git@github.com
    ```

19. **Generate SSH Key**:
    If you need to regenerate an SSH key:
    ```powershell
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
    ```

20. **Add SSH Key to SSH Agent**:
    After generating your SSH key, add it to the SSH agent:
    ```powershell
    ssh-add ~/.ssh/id_rsa
    ```

21. **List SSH Keys**:
    To list the SSH keys added to your SSH agent:
    ```powershell
    ssh-add -l
    ```

22. **Open Git Configuration File**:
    To open the global Git configuration file in a text editor:
    ```powershell
    notepad.exe $env:USERPROFILE\.gitconfig
    ```

---

### **PowerShell System Commands**

1. **List Files in a Directory**:
   List all files in the current directory:
   ```powershell
   Get-ChildItem
   ```

2. **Change Directory**:
   Navigate to a different directory:
   ```powershell
   Set-Location -Path "C:\path\to\directory"
   ```

3. **Clear the Console**:
   Clear the terminal screen:
   ```powershell
   Clear-Host
   ```

4. **Check Current Directory**:
   Get the current directory:
   ```powershell
   Get-Location
   ```

5. **Create a New Directory**:
   Create a new folder:
   ```powershell
   New-Item -ItemType Directory -Name "NewFolder"
   ```

6. **Remove a File**:
   Delete a specific file:
   ```powershell
   Remove-Item "filename.txt"
   ```

7. **Remove a Directory**:
   Delete a directory:
   ```powershell
   Remove-Item "DirectoryName" -Recurse
   ```

8. **Rename a File**:
   Rename a file:
   ```powershell
   Rename-Item "oldname.txt" "newname.txt"
   ```

9. **Copy a File**:
   Copy a file:
   ```powershell
   Copy-Item "sourcefile.txt" "destinationfile.txt"
   ```

10. **Move a File**:
    Move a file to a different directory:
    ```powershell
    Move-Item "sourcefile.txt" "C:\new\path"
    ```

---

### **Git-Related Troubleshooting Commands**

1. **View SSH Configuration**:
   To view your SSH configuration settings:
   ```powershell
   cat ~/.ssh/config
   ```

2. **Check Git Remotes**:
   To check the remotes for your Git repository:
   ```powershell
   git remote show origin
   ```

3. **Check for Conflicts**:
   If you encounter merge conflicts, you can check the status:
   ```powershell
   git status
   ```

---

### **Summary**

These are common **PowerShell commands** that you can use to work with Git and GitHub on **Windows**. You can perform almost all Git-related operations from PowerShell, as well as handle system tasks like navigating directories and managing files.

Let me know if you need help with a specific command or if you'd like more detailed explanations!