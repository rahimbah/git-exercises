`git rebase --onto` allows you to move a branch to a different place.

That:
```
git rebase issue-555 --onto your-master
```
means:

> Get all commits that are not in issue-555 and place them onto your-master branch.

It is consistent with regular rebase (`--onto` defaults to branch you are rebasing to), i.e.:
`git rebase issue-555`
means: Get all commits that are not in issue-555 and place them onto issue-555.

More info: http://git-scm.com/book/en/v2/Git-Branching-Rebasing#More-Interesting-Rebases