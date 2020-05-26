# Git Aliases on .gitconfig file

First, install **Git** on your machine :
`sudo apt-get install git`

Create your .gitconfig file :
`touch ~/.gitconfig`

Install **Nano** on your machine :
`sudo apt install nano`

For to edit your identity :
`git config --global user.name "Foo Bar"`
`git config --global user.email "foobar@baz.com"`

*For more informations or more git commands, read the [official documentation](https://git-scm.com/doc)*

*These aliases aren't official*

    [core]
        editor = nano

    [user]
        email = foobar@baz.com
        name = Foo Bar

    [push]
        default = simple

    [alias]
        i = !git init
        cl = !git clone
        df = !git diff
        rs = !git reset
        shame = !git blame --show-name --show-number --show-email
        rmta = !git remote add
        sts = !git status
        ckb = !git checkout -b
        ck = !git checkout
        ckd = !git checkout develop
        ckm = !git checkout master
        ada = !git add -A
        cmt = !git commit -m
        amend = !git commit --amend
        ps = !git push
        psf = !git push -f
        psu = !git push -u
        wip = !git add -A && git commit -m "feature: wip" && git push
        pl = !git pull
        t = !git tag
        m = !git merge
        sm = !git merge --squash
        rbi = !git rebase -i
        ssh = !git stash
        sshl = !git stash list
        sshp = !git stash pop
        sshd = !git stash drop
        sshc = !git stash clear
        b = !git branch
        bc = !git branch -D
        graph = !git log --graph --decorate --oneline --color=always
