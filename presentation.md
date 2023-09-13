# Git Config

```
git config --global core.excludesfile $HOME/.gitignore

git config --global core.editor nvim
git config --global core.editor "code --wait"

git config --global core.ignorecase false

git config --global push.defaut current
# https://git-scm.com/docs/git-push#Documentation/git-push.txt-pushdefault

git config --global pull.rebase true

git config --global rebase.autostash true
git config --global rebase.autosquash true
git config --global rerere.enabled true

```

# Rebase
```
git checkout -b feature/update-user

edit user.rb

git status
git add user.rb
git commit --messsage 'Update readme'
git push

[Open PR]
[Change requests]

git commit --message 'Fix PRs'
git push

git fetch
git rebase --interactive master
git mergetool
git rebase --continue
git push --force-with-lease
```

# Why rebase instead of merge?

Hej stef, we are using squash and merge so it does not matter. True but.
With `git merge master` within a feature branch you are introducing addittional changes to fix merge conflicts, but you do them for the whole
base branch, not by the individual commits.
Rebase gives us a nicer history and easier to follow PRs

# References
https://git-scm.com/docs/git-config
https://github.com/so-fancy/diff-so-fancy
https://github.com/jesseduffield/lazygit
