# 675_phase2_project

## Git Branching 101:

    ilya.kopyl@ilyakopyl-ltm 675_phase2_project (master)$ git branch
    * master


    ilya.kopyl@ilyakopyl-ltm 675_phase2_project (master)$ git branch dev-ilya

    
    ilya.kopyl@ilyakopyl-ltm 675_phase2_project (master)$ git branch
      dev-ilya
    * master

    
    ilya.kopyl@ilyakopyl-ltm 675_phase2_project (master)$ git checkout dev-ilya
    Switched to branch 'dev-ilya'

    
    ilya.kopyl@ilyakopyl-ltm 675_phase2_project (dev-ilya)$ git branch
    * dev-ilya
      master

    
    ilya.kopyl@ilyakopyl-ltm 675_phase2_project (dev-ilya)*$ git status
    On branch dev-ilya
    Changes not staged for commit:
      (use "git add <file>..." to update what will be committed)
      (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   README.md

    Untracked files:
      (use "git add <file>..." to include in what will be committed)

        .gitignore

    no changes added to commit (use "git add" and/or "git commit -a")


    ilya.kopyl@ilyakopyl-ltm 675_phase2_project (dev-ilya)*$ git add .gitignore 


    ilya.kopyl@ilyakopyl-ltm 675_phase2_project (dev-ilya)*$ git status
    On branch dev-ilya
    Changes to be committed:
      (use "git reset HEAD <file>..." to unstage)

        new file:   .gitignore

    Changes not staged for commit:
      (use "git add <file>..." to update what will be committed)
      (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   README.md


    ilya.kopyl@ilyakopyl-ltm 675_phase2_project (dev-ilya)*$ git commit -m "Added .gitignore"
    [dev-ilya dbc9917] Added .gitignore
     1 file changed, 1 insertion(+)
     create mode 100644 .gitignore


    ilya.kopyl@ilyakopyl-ltm 675_phase2_project (dev-ilya)*$ git add README.md


    ilya.kopyl@ilyakopyl-ltm 675_phase2_project (dev-ilya)*$ git status
    On branch dev-ilya
    Changes to be committed:
      (use "git reset HEAD <file>..." to unstage)

        modified:   README.md


    ilya.kopyl@ilyakopyl-ltm 675_phase2_project (dev-ilya)*$ git commit -m "Modified README"
     26
    [dev-ilya 43f365b] Modified README
     1 file changed, 18 insertions(+), 1 deletion(-)
     rewrite README.md (100%)


    ilya.kopyl@ilyakopyl-ltm 675_phase2_project (dev-ilya)$ git status
    On branch dev-ilya
    nothing to commit, working tree clean
    ilya.kopyl@ilyakopyl-ltm 675_phase2_project (dev-ilya)$ git push origin dev-ilya
    Enumerating objects: 8, done.
    Counting objects: 100% (8/8), done.
    Delta compression using up to 8 threads
    Compressing objects: 100% (5/5), done.
    Writing objects: 100% (6/6), 1.44 KiB | 1.44 MiB/s, done.
    Total 6 (delta 0), reused 0 (delta 0)
    remote:
    remote: Create a pull request for 'dev-ilya' on GitHub by visiting:
    remote:      https://github.com/ikopyl/675_phase2_project/pull/new/dev-ilya
    remote:
    To github.com:ikopyl/675_phase2_project.git
     * [new branch]      dev-ilya -> dev-ilya


