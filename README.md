PS E:\gitlearn> cd intern-portfolio     
PS E:\gitlearn\intern-portfolio> git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:
        modified:   index.html

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    About.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        About.md
        note.txt

PS E:\gitlearn\intern-portfolio> git init
Reinitialized existing Git repository in E:/gitlearn/intern-portfolio/.git/
PS E:\gitlearn\intern-portfolio> git remote add origin https://github.com/VrajNakum/intern-portfolio.git          
error: remote origin already exists.
PS E:\gitlearn\intern-portfolio> git branch
  feature-update
* main
PS E:\gitlearn\intern-portfolio> git merge Feature-update
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.
PS E:\gitlearn\intern-portfolio> git commit -m "merge Feature-update"                
[main ce907e4] merge Feature-update
PS E:\gitlearn\intern-portfolio> git merge Feature-update            
Already up to date.
PS E:\gitlearn\intern-portfolio> git push -u origin main                             
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 16 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 668 bytes | 668.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/VrajNakum/intern-portfolio.git
   cd77cd2..ce907e4  main -> main
branch 'main' set up to track 'origin/main'.
PS E:\gitlearn\intern-portfolio> git branch feature-Contact                          
PS E:\gitlearn\intern-portfolio> git branch                
  feature-Contact
  feature-update
* main
PS E:\gitlearn\intern-portfolio> git add Contact.txt
PS E:\gitlearn\intern-portfolio> git commit -m "this is my Contact file"
[main 2da675f] this is my Contact file
 1 file changed, 1 insertion(+)
 create mode 100644 Contact.txt
PS E:\gitlearn\intern-portfolio> git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    About.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        About.md
        note.txt

no changes added to commit (use "git add" and/or "git commit -a")
PS E:\gitlearn\intern-portfolio> git init 
Reinitialized existing Git repository in E:/gitlearn/intern-portfolio/.git/
PS E:\gitlearn\intern-portfolio> git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    About.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        About.md
        note.txt

no changes added to commit (use "git add" and/or "git commit -a")
PS E:\gitlearn\intern-portfolio> git log
commit 2da675f024ce7c5375445505c524f3cf02278bb6 (HEAD -> main)
Author: Vraj <vrajnakum11@gmail.com>
Date:   Thu Aug 13 15:10:20 2026 +0530

    this is my Contact file

commit ce907e4f78f44264f8eb2b16da2a2b927952056e (origin/main, feature-Contact)
Merge: 51d9bee eaedd55
Author: Vraj <vrajnakum11@gmail.com>
Date:   Thu Aug 13 15:06:38 2026 +0530

    merge Feature-update

commit eaedd55c36ee39a6d670df6515be4fa6e0c10c6e (origin/feature-update, feature-update)
Author: Vraj <vrajnakum11@gmail.com>
Date:   Thu Aug 13 14:57:23 2026 +0530

    this is my Change in index and about in the branch feature-update

commit 51d9bee91ef8545bc885ec27c66f4eeb693fa56a
Author: Vraj <vrajnakum11@gmail.com>
PS E:\gitlearn\intern-portfolio> git switch feature-Contact                          
D       About.txt  
Switched to branch 'feature-Contact'
PS E:\gitlearn\intern-portfolio> git branch
* feature-Contact
  feature-update
  main
PS E:\gitlearn\intern-portfolio> git add Contact.txt                    
fatal: pathspec 'Contact.txt' did not match any files
PS E:\gitlearn\intern-portfolio> git commit -m "this is my Contact file"
On branch feature-Contact
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    About.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        About.md
        note.txt

no changes added to commit (use "git add" and/or "git commit -a")
PS E:\gitlearn\intern-portfolio> git log
commit ce907e4f78f44264f8eb2b16da2a2b927952056e (HEAD -> feature-Contact, origin/main)
Merge: 51d9bee eaedd55
Author: Vraj <vrajnakum11@gmail.com>
Date:   Thu Aug 13 15:06:38 2026 +0530

    merge Feature-update

commit eaedd55c36ee39a6d670df6515be4fa6e0c10c6e (origin/feature-update, feature-update)
Author: Vraj <vrajnakum11@gmail.com>
Date:   Thu Aug 13 14:57:23 2026 +0530

    this is my Change in index and about in the branch feature-update

commit 51d9bee91ef8545bc885ec27c66f4eeb693fa56a
Author: Vraj <vrajnakum11@gmail.com>
Date:   Thu Aug 13 14:52:06 2026 +0530

    this is my Change in index and about

commit cd77cd24d748847a01ed2d7d70113d83404acee1
PS E:\gitlearn\intern-portfolio> git add Contact.txt                     
fatal: pathspec 'Contact.txt' did not match any files
PS E:\gitlearn\intern-portfolio> git init
Reinitialized existing Git repository in E:/gitlearn/intern-portfolio/.git/
PS E:\gitlearn\intern-portfolio> git add Contact.txt
fatal: pathspec 'Contact.txt' did not match any files
PS E:\gitlearn\intern-portfolio> git status
On branch feature-Contact
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    About.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        About.md
        note.txt

no changes added to commit (use "git add" and/or "git commit -a")
PS E:\gitlearn\intern-portfolio> git add Contact.txt
fatal: pathspec 'Contact.txt' did not match any files
PS E:\gitlearn\intern-portfolio> git commit -m "this is my Contact file"
On branch feature-Contact
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    About.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        About.md
        note.txt

no changes added to commit (use "git add" and/or "git commit -a")
PS E:\gitlearn\intern-portfolio> git init
Reinitialized existing Git repository in E:/gitlearn/intern-portfolio/.git/
PS E:\gitlearn\intern-portfolio> git status
On branch feature-Contact
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    About.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        About.md
        note.txt

no changes added to commit (use "git add" and/or "git commit -a")
PS E:\gitlearn\intern-portfolio> git init
Reinitialized existing Git repository in E:/gitlearn/intern-portfolio/.git/
PS E:\gitlearn\intern-portfolio> git push -u origin Feature-contact     
fatal: Feature-contact cannot be resolved to branch
PS E:\gitlearn\intern-portfolio> git branch
* feature-Contact
  feature-update
  main
PS E:\gitlearn\intern-portfolio> git status
On branch feature-Contact
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    About.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        About.md
        note.txt

no changes added to commit (use "git add" and/or "git commit -a")
PS E:\gitlearn\intern-portfolio> git add .
PS E:\gitlearn\intern-portfolio> git status
On branch feature-Contact
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   About.md
        deleted:    About.txt
        new file:   note.txt

PS E:\gitlearn\intern-portfolio> git status
On branch feature-Contact
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   About.md
        deleted:    About.txt
        new file:   note.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Contact.txt

PS E:\gitlearn\intern-portfolio> git add Contact.txt 
PS E:\gitlearn\intern-portfolio> git commit -m "this is my Contact file"
[feature-Contact d8f7b75] this is my Contact file
 4 files changed, 1 insertion(+), 5 deletions(-)
 create mode 100644 About.md
 delete mode 100644 About.txt
 create mode 100644 Contact.txt
 create mode 100644 note.txt
PS E:\gitlearn\intern-portfolio> git status
On branch feature-Contact
nothing to commit, working tree clean
PS E:\gitlearn\intern-portfolio> git push -u origin Feature-contact     
fatal: Feature-contact cannot be resolved to branch
PS E:\gitlearn\intern-portfolio> git commit -m "this is push to branch of the contact"
On branch feature-Contact
nothing to commit, working tree clean
PS E:\gitlearn\intern-portfolio> git push -u origin Feature-contact                  
fatal: Feature-contact cannot be resolved to branch
PS E:\gitlearn\intern-portfolio> git log
commit d8f7b7580fe6e5790d365d9a53aeefca6f406f9f (HEAD -> feature-Contact)
Author: Vraj <vrajnakum11@gmail.com>
Date:   Thu Aug 13 15:17:44 2026 +0530

    this is my Contact file

commit ce907e4f78f44264f8eb2b16da2a2b927952056e (origin/main)
Merge: 51d9bee eaedd55
Author: Vraj <vrajnakum11@gmail.com>
Date:   Thu Aug 13 15:06:38 2026 +0530

    merge Feature-update

commit eaedd55c36ee39a6d670df6515be4fa6e0c10c6e (origin/feature-update, feature-update)
Author: Vraj <vrajnakum11@gmail.com>
Date:   Thu Aug 13 14:57:23 2026 +0530

    this is my Change in index and about in the branch feature-update

commit 51d9bee91ef8545bc885ec27c66f4eeb693fa56a
Author: Vraj <vrajnakum11@gmail.com>
PS E:\gitlearn\intern-portfolio> git switch main                                     
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
PS E:\gitlearn\intern-portfolio> git branch     
  feature-Contact
  feature-update
* main
PS E:\gitlearn\intern-portfolio> git push -u origin main                             
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 365 bytes | 365.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/VrajNakum/intern-portfolio.git
   ce907e4..2da675f  main -> main
branch 'main' set up to track 'origin/main'.
PS E:\gitlearn\intern-portfolio> 
