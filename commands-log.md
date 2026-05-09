## Task 1

```bash
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework> git init
Initialized empty Git repository in C:/Users/jacob/Files/Programming/VsCode/fullstack-genai-05-homework/.git/
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework> git add .
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework> git commit -m "Create index.html"
[master (root-commit) a5fd3b0] Create index.html
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.html
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework> git restore index.html
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework> git add .
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework> git rm --cached passwords.txt
rm 'passwords.txt'
```

## Task 2

```bash
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework>
 *  History restored

PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework> git branch -M main
>> git remote add origin https://github.com/JeStdGit/Homework-05.git
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework> git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 214 bytes | 214.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/JeStdGit/Homework-05.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
```

## Task 3

**Second Programmer's pc:**

```bash
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework-clone> git clone https://github.com/JeStdGit/Homework-05
Cloning into 'Homework-05'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.
```

**Teammate's pc:**

```bash
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework> git add .
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework> git commit -m "new edit from the teammate"
[main 11faee9] new edit from the teammate
 2 files changed, 11 insertions(+)
 create mode 100644 passwords.txt
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 20 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 456 bytes | 228.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/JeStdGit/Homework-05.git
   a5fd3b0..11faee9  main -> main
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework>
```

**Second Programmer's pc:**

```bash
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework-clone> git pull
fatal: not a git repository (or any of the parent directories): .git
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework-clone> cd .\Homework-05\
PS C:\Users\jacob\Files\Programming\VsCode\fullstack-genai-05-homework-clone\Homework-05> git pull
Updating a5fd3b0..11faee9
Fast-forward
 index.html    | 11 +++++++++++
 passwords.txt |  0
 2 files changed, 11 insertions(+)
 create mode 100644 passwords.txt
```
