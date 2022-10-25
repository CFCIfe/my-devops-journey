## Output of the following commands

---

### git config -l

```
user.name=Peter Abolude
user.email=aboludepeter@gmail.com
credential.helper=store
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.postbuffer=524288000
core.repositoryformatversion=0
core.filemode=true
core.bare=false
core.logallrefupdates=true
remote.origin.url=git@github.com:CFCIfe/altschool-cloud-exercises.git
remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*
branch.master.remote=origin
branch.master.merge=refs/heads/master
```
---

### git remote -v

```
origin	git@github.com:CFCIfe/altschool-cloud-exercises.git (fetch)
origin	git@github.com:CFCIfe/altschool-cloud-exercises.git (push)
```

---

### git log

```
commit 162c9ceda4eb62dcaccbb057b3a30dff5915ab19 (HEAD -> master, origin/master)
Author: Peter Abolude <aboludepeter@gmail.com>
Date:   Wed Aug 31 18:35:45 2022 +0100

    exercise 4

commit b6875e10631b1ee4b29f6ffe3bf37a7d6ae20650
Author: Peter Abolude <aboludepeter@gmail.com>
Date:   Mon Aug 29 22:07:16 2022 +0100

    Submit Exercise 3

commit a98895ac889216e376b343e1b48a4feebdd181cd
Author: Peter Abolude <aboludepeter@gmail.com>
Date:   Thu Aug 25 11:18:41 2022 +0100

    file name change

commit cd2d1d8962215372345fe4bf2f4a3ec5f27b7f06
Author: Peter Abolude <aboludepeter@gmail.com>
Date:   Tue Aug 16 21:31:23 2022 +0100

    Exercise one and Two

commit fc9d3110f65ecbb43d56fec0b751ca25bab3f3f2
Author: Peter Abolude <aboludepeter@gmail.com>
Date:   Tue Aug 16 18:29:42 2022 +0100

    first push
```