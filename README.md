
# **GIT COMPLETE NOTES WITH COMMAND + OUTPUT**

---

##  1. Check Git Version

###  Command:

```bash
git --version
```

###  Output:

```text
git version 2.44.0.windows.1
```

---

##  2. Set Git Username

###  Command:

```bash
git config --global user.name "Omkar Shinde"
```

###  Output:

```text
(no output – command executed successfully)
```

---

##  3. Set Git Email

###  Command:

```bash
git config --global user.email "shindeomkar2508@gmail.com"
```

###  Output:

```text
(no output – command executed successfully)
```

---

##  4. Verify Git Configuration

###  Command:

```bash
git config --list
```

###  Output:

```text
user.name=Omkar Shinde
user.email=shindeomkar2508@gmail.com
```

---

##  5. Create Project Folder

###  Command:

```bash
mkdir Gitdemo
cd Gitdemo
```

###  Output:

```text
Directory created and moved inside Gitdemo
```

---

##  6. Initialize Git Repository

###  Command:

```bash
git init
```

###  Output:

```text
Initialized empty Git repository in C:/Users/.../Gitdemo/.git/
```

---

##  7. Check Status

###  Command:

```bash
git status
```

###  Output:

```text
On branch master
No commits yet
nothing to commit
```

---

##  8. Create Files

Create manually:

```text
hello.html
hello.py
```

---

##  9. Add Files to Staging

###  Command:

```bash
git add .
```

###  Output:

```text
(no output)
```

---

##  10. First Commit

###  Command:

```bash
git commit -m "Initial commit"
```

###  Output:

```text
[master (root-commit) a12b67c] Initial commit
 2 files changed
 create mode 100644 hello.html
 create mode 100644 hello.py
```

---

##  11. Create New Branch

###  Command:

```bash
git branch design
```

###  Output:

```text
(no output)
```

---

##  12. View Branches

###  Command:

```bash
git branch
```

###  Output:

```text
  design
* master
```

---

##  13. Switch to Design Branch

###  Command:

```bash
git checkout design
```

###  Output:

```text
Switched to branch 'design'
```

---

##  14. Modify File (hello.py)

Edit file and save.

---

##  15. Add & Commit in Design Branch

###  Commands:

```bash
git add .
git commit -m "Updated hello.py"
```

###  Output:

```text
[design 3ec091d] Updated hello.py
 1 file changed, 1 insertion(+)
```

---

##  16. Switch to Master Branch

###  Command:

```bash
git checkout master
```

###  Output:

```text
Switched to branch 'master'
```

---

##  17. Merge Design into Master

###  Command:

```bash
git merge design
```

###  Output:

```text
Updating a12b67c..3ec091d
Fast-forward
 hello.py | 1 +
 1 file changed, 1 insertion(+)
```

---

##  18. Add GitHub Remote

###  Command:

```bash
git remote add origin https://github.com/omkarshinde25/Git-Push-Pull-Demo.git
```

###  Output:

```text
(no output)
```

 If error comes:

```text
error: remote origin already exists.
```

 Fix:

```bash
git remote set-url origin https://github.com/omkarshinde25/Git-Push-Pull-Demo.git
```

---

##  19. Push Master Branch to GitHub

###  Command:

```bash
git push -u origin master
```

###  Output:

```text
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Writing objects: 100% (3/3), done.
To github.com/omkarshinde25/Git-Push-Pull-Demo.git
 * [new branch] master -> master
```

---

##  20. Push Design Branch to GitHub

###  Command:

```bash
git push -u origin design
```

###  Output:

```text
To github.com/omkarshinde25/Git-Push-Pull-Demo.git
 * [new branch] design -> design
```

---

##  21. View Commit History

###  Command:

```bash
git log --oneline
```

###  Output:

```text
3ec091d Updated hello.py
a12b67c Initial commit
```

---

##  22. Delete Branch After Merge (Optional)

###  Command:

```bash
git branch -d design
```

###  Output:

```text
Deleted branch design (was 3ec091d).
```

---

#  **FULL GIT PROCESS COMPLETE**

Git Config → Init → Add → Commit → Branch → Checkout → Merge → Push → DONE


