# Lesson2
Net Devops HW Les 2

New data Step 7

Terraform git ignore

exclude files:
    *.tfstate  
    *.tfstate.*  
    crash.log
   *.tfvars
   override.tf
    override.tf.json
    *_override.tf
    *_override.tf.json

    .terraformrc
    terraform.rc

----------------------
Выводы команд домашнего задания 3 до пункта 7

1-9 part 1 gitlab

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git remote -v
origin  https://github.com/olegrovenskiy/Lesson2 (fetch)
origin  https://github.com/olegrovenskiy/Lesson2 (push)

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git remote add gitlab https://gitlab.com/olegrovenskiy/devops-netology

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git remote -v
gitlab  https://gitlab.com/olegrovenskiy/devops-netology (fetch)
gitlab  https://gitlab.com/olegrovenskiy/devops-netology (push)
origin  https://github.com/olegrovenskiy/Lesson2 (fetch)
origin  https://github.com/olegrovenskiy/Lesson2 (push)

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git push -u gitlab main
warning: redirecting to https://gitlab.com/olegrovenskiy/devops-netology.git/
Enumerating objects: 44, done.
Counting objects: 100% (44/44), done.
Delta compression using up to 4 threads
Compressing objects: 100% (32/32), done.
Writing objects: 100% (44/44), 4.51 KiB | 355.00 KiB/s, done.
Total 44 (delta 13), reused 3 (delta 0), pack-reused 0
To https://gitlab.com/olegrovenskiy/devops-netology
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'gitlab'.

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git remote -v
gitlab  https://gitlab.com/olegrovenskiy/devops-netology (fetch)
gitlab  https://gitlab.com/olegrovenskiy/devops-netology (push)
origin  https://github.com/olegrovenskiy/Lesson2 (fetch)
origin  https://github.com/olegrovenskiy/Lesson2 (push)

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>


--------------------

point 1-9 step 2 bitbucket


(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git push -u bitbucket main
Enumerating objects: 44, done.
Counting objects: 100% (44/44), done.
Delta compression using up to 4 threads
Compressing objects: 100% (32/32), done.
Writing objects: 100% (44/44), 4.51 KiB | 462.00 KiB/s, done.
Total 44 (delta 13), reused 3 (delta 0), pack-reused 0
remote:
remote: Create pull request for main:
remote:   https://bitbucket.org/olegrovenskiy/devops-netology/pull-requests/new?source=main&t=1
remote:
To https://bitbucket.org/olegrovenskiy/devops-netology/src/master/
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'bitbucket'.

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>

--------------------

Light tag



(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git tag

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git tag v0.1

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git tag
v0.1

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git show v0.1
commit ba15f51e523b1e0e93a1dfb5b580b1bd1cd06109 (HEAD -> main, tag: v0.1, origin/main, origin/HEAD, gitlab/main, bitbucket/main)
Author: oleg.rovenskiy <roleg_n@mail.ru>
Date:   Sun May 9 13:12:33 2021 +0300

    After delete and Move 2

diff --git a/test2.txt b/test2.txt
deleted file mode 100644
index cb994f2..0000000
--- a/test2.txt
+++ /dev/null
@@ -1,3 +0,0 @@
-one more test
-
-1 2 3 

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git remote -v
bitbucket       https://bitbucket.org/olegrovenskiy/devops-netology/src/master/ (fetch)
bitbucket       https://bitbucket.org/olegrovenskiy/devops-netology/src/master/ (push)
gitlab  https://gitlab.com/olegrovenskiy/devops-netology (fetch)
gitlab  https://gitlab.com/olegrovenskiy/devops-netology (push)
origin  https://github.com/olegrovenskiy/Lesson2 (fetch)
origin  https://github.com/olegrovenskiy/Lesson2 (push)

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git push origin --tags
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/olegrovenskiy/Lesson2
 * [new tag]         v0.1 -> v0.1

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git push gitlab --tags
warning: redirecting to https://gitlab.com/olegrovenskiy/devops-netology.git/
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://gitlab.com/olegrovenskiy/devops-netology
 * [new tag]         v0.1 -> v0.1

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git push bitbucket --tags
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://bitbucket.org/olegrovenskiy/devops-netology/src/master/
 * [new tag]         v0.1 -> v0.1

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>

-----------

Anat tag

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git tag -a v0.2 -m "Ann Tag"

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git tag
v0.1
v0.2

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git show v0.2
tag v0.2
Tagger: oleg.rovenskiy <roleg_n@mail.ru>
Date:   Fri May 14 09:42:47 2021 +0300

Ann Tag

commit ba15f51e523b1e0e93a1dfb5b580b1bd1cd06109 (HEAD -> main, tag: v0.2, tag: v0.1, origin/main, origin/HEAD, gitlab/main, bitbucket/main)
Author: oleg.rovenskiy <roleg_n@mail.ru>
Date:   Sun May 9 13:12:33 2021 +0300

    After delete and Move 2

diff --git a/test2.txt b/test2.txt
deleted file mode 100644
index cb994f2..0000000
--- a/test2.txt
+++ /dev/null
@@ -1,3 +0,0 @@
-one more test
-
-1 2 3 

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git push bitbucket --tags
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 160 bytes | 80.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://bitbucket.org/olegrovenskiy/devops-netology/src/master/
 * [new tag]         v0.2 -> v0.2

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git push gitlab --tags
warning: redirecting to https://gitlab.com/olegrovenskiy/devops-netology.git/
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 160 bytes | 80.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://gitlab.com/olegrovenskiy/devops-netology
 * [new tag]         v0.2 -> v0.2

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git push origin --tags
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 160 bytes | 80.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/olegrovenskiy/Lesson2
 * [new tag]         v0.2 -> v0.2

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>


------------------------

Task 3

commit 4b8bd582e04a4f589084ca8164f6dd7aa67179e5
Author: oleg.rovenskiy <roleg_n@mail.ru>
Date:   Sun May 9 11:18:18 2021 +0300

    Prepare to Delete and move

----------

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git checkout 4b8bd582e04a4f589084ca8164f6dd7aa67179e5
Note: switching to '4b8bd582e04a4f589084ca8164f6dd7aa67179e5'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 4b8bd58 Prepare to Delete and move

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git switch -c fix
Switched to a new branch 'fix'

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>git push -u origin fix
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'fix' on GitHub by visiting:
remote:      https://github.com/olegrovenskiy/Lesson2/pull/new/fix
remote:
To https://github.com/olegrovenskiy/Lesson2
 * [new branch]      fix -> fix
Branch 'fix' set up to track remote branch 'fix' from 'origin'.

(venv) C:\Users\Олег\PycharmProjects\New_Netology\Lesson2>


---------------

task 4 визуальный редактор

1 2 3 4




