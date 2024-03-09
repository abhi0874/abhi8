# abhi8
C:\Users\admin>cd C:\ai59\gitlab\expv8

C:\ai59\gitlab\expv8>git init
Initialized empty Git repository in C:/ai59/gitlab/expv8/.git/

C:\ai59\gitlab\expv8>eds.txt

C:\ai59\gitlab\expv8>git log
fatal: your current branch 'master' does not have any commits yet

C:\ai59\gitlab\expv8>eds.txt

C:\ai59\gitlab\expv8>git add eds.txt

C:\ai59\gitlab\expv8>git commit -m "com1"
[master (root-commit) 2e887d0] com1
 1 file changed, 2 insertions(+)
 create mode 100644 eds.txt

C:\ai59\gitlab\expv8>eds.txt

C:\ai59\gitlab\expv8>git add eds.txt

C:\ai59\gitlab\expv8>git commit -m "com2"
[master d062d5f] com2
 1 file changed, 2 insertions(+), 1 deletion(-)

C:\ai59\gitlab\expv8>eds.txt

C:\ai59\gitlab\expv8>git add eds.txt

C:\ai59\gitlab\expv8>git commit -m "com2"
[master 265e869] com2
 1 file changed, 1 insertion(+)

C:\ai59\gitlab\expv8>eds.txt

C:\ai59\gitlab\expv8>git add eds.txt

C:\ai59\gitlab\expv8>git commit -m "com3"
[master 2089e4b] com3
 1 file changed, 2 insertions(+), 1 deletion(-)

C:\ai59\gitlab\expv8>git log
commit 2089e4b9ae525a2cf448e1a73bf773de64c4e078 (HEAD -> master)
Author: suraj-6 <suraj.204214@gmail.com>
Date:   Sat Mar 9 08:26:23 2024 +0530

    com3

commit 265e869e9570d11456b6f205797cdf9a0bb5fa56
Author: suraj-6 <suraj.204214@gmail.com>
Date:   Sat Mar 9 08:26:01 2024 +0530

    com2

commit d062d5fa9811cc8e1dfb67753d244f54beea89ad
Author: suraj-6 <suraj.204214@gmail.com>
Date:   Sat Mar 9 08:25:27 2024 +0530

    com2

commit 2e887d0b7866ae1d9542fec603142626473a54a9
Author: suraj-6 <suraj.204214@gmail.com>
Date:   Sat Mar 9 08:24:53 2024 +0530

    com1

C:\ai59\gitlab\expv8>git cherry-pick  2089e4b9ae525a2cf448e1a73bf773de64c4e078 ^.. 2e887d0b7866ae1d9542fec603142626473a54a9
error: empty commit set passed
fatal: cherry-pick failed

C:\ai59\gitlab\expv8>git cherry-pick 2089e4b9ae525a2cf448e1a73bf773de64c4e078 ^.. 2e887d0b7866ae1d9542fec603142626473a54a9
error: empty commit set passed
fatal: cherry-pick failed

C:\ai59\gitlab\expv8>git checkout master
Already on 'master'

C:\ai59\gitlab\expv8>git cherry-pick 2089e4b9ae525a2cf448e1a73bf773de64c4e078 ^.. 2e887d0b7866ae1d9542fec603142626473a54a9
error: empty commit set passed
fatal: cherry-pick failed

C:\ai59\gitlab\expv8>git cherry-pick 2e887d0b7866ae1d9542fec603142626473a54a9 ^.. 2e887d0b7866ae1d9542fec603142626473a54a9
error: empty commit set passed
fatal: cherry-pick failed

C:\ai59\gitlab\expv8>git cherry-pick <2e887d0b7866ae1d9542fec603142626473a54a9> ^.. <2e887d0b7866ae1d9542fec603142626473a54a9>
The syntax of the command is incorrect.

C:\ai59\gitlab\expv8>git cherry-pick 2e887d0b7866ae1d9542fec603142626473a54a9 ^.. 2e887d0b7866ae1d9542fec603142626473a54a9
error: empty commit set passed
fatal: cherry-pick failed

C:\ai59\gitlab\expv8>git tag v1.0

C:\ai59\gitlab\expv8>git log
commit 2089e4b9ae525a2cf448e1a73bf773de64c4e078 (HEAD -> master, tag: v1.0)
Author: suraj-6 <suraj.204214@gmail.com>
Date:   Sat Mar 9 08:26:23 2024 +0530

    com3

commit 265e869e9570d11456b6f205797cdf9a0bb5fa56
Author: suraj-6 <suraj.204214@gmail.com>
Date:   Sat Mar 9 08:26:01 2024 +0530

    com2

commit d062d5fa9811cc8e1dfb67753d244f54beea89ad
Author: suraj-6 <suraj.204214@gmail.com>
Date:   Sat Mar 9 08:25:27 2024 +0530

    com2

commit 2e887d0b7866ae1d9542fec603142626473a54a9
Author: suraj-6 <suraj.204214@gmail.com>
Date:   Sat Mar 9 08:24:53 2024 +0530

    com1

C:\ai59\gitlab\expv8>git cherry-pick  2089e4b9ae525a2cf448e1a73bf773de64c4e078 ^.. 2e887d0b7866ae1d9542fec603142626473a54a9
error: empty commit set passed
fatal: cherry-pick failed

C:\ai59\gitlab\expv8>git checkout master
Already on 'master'

C:\ai59\gitlab\expv8>git checkout -b tb
Switched to a new branch 'tb'

C:\ai59\gitlab\expv8>git cherry-pick  2089e4b9ae525a2cf448e1a73bf773de64c4e078 ^.. 2e887d0b7866ae1d9542fec603142626473a54a9
error: empty commit set passed
fatal: cherry-pick failed

C:\ai59\gitlab\expv8>git cherry-pick 2089e4b9ae525a2cf448e1a73bf773de64c4e078 ^.. 2e887d0b7866ae1d9542fec603142626473a54a9
error: empty commit set passed
fatal: cherry-pick failed

C:\ai59\gitlab\expv8>git cherry-pick 2e887d0b7866ae1d9542fec603142626473a54a9 ^.. 2e887d0b7866ae1d9542fec603142626473a54a9
error: empty commit set passed
fatal: cherry-pick failed

C:\ai59\gitlab\expv8>git log -n 2
commit 2089e4b9ae525a2cf448e1a73bf773de64c4e078 (HEAD -> tb, tag: v1.0, master)
Author: suraj-6 <suraj.204214@gmail.com>
Date:   Sat Mar 9 08:26:23 2024 +0530

    com3

commit 265e869e9570d11456b6f205797cdf9a0bb5fa56
Author: suraj-6 <suraj.204214@gmail.com>
Date:   Sat Mar 9 08:26:01 2024 +0530

    com2

C:\ai59\gitlab\expv8>git log -n 3
commit 2089e4b9ae525a2cf448e1a73bf773de64c4e078 (HEAD -> tb, tag: v1.0, master)
Author: suraj-6 <suraj.204214@gmail.com>
Date:   Sat Mar 9 08:26:23 2024 +0530

    com3

commit 265e869e9570d11456b6f205797cdf9a0bb5fa56
Author: suraj-6 <suraj.204214@gmail.com>
Date:   Sat Mar 9 08:26:01 2024 +0530

    com2

commit d062d5fa9811cc8e1dfb67753d244f54beea89ad
Author: suraj-6 <suraj.204214@gmail.com>
Date:   Sat Mar 9 08:25:27 2024 +0530

    com2

C:\ai59\gitlab\expv8>git revert  2089e4b9ae525a2cf448e1a73bf773de64c4e078
[tb 95cd229] Revert "com3"
 1 file changed, 1 insertion(+), 2 deletions(-)
