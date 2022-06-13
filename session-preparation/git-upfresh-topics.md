# git upfresh - Conference session preparation

## Topics for the confrence talk

* git stash (possible with link to stashing partially staged changes) (<https://github.blog/2022-01-24-highlights-from-git-2-35/>)
* git sparse checkout (<https://github.blog/2021-11-15-highlights-from-git-2-34/>)
* ort merge algorithm
* replace a single commit (amend) with fixup

´´´ shell
marko@hp-lx:~/projects/git$ git commit --fixup=amend:6e158
[main d320976] amend! Three
marko@hp-lx:~/projects/git$ git rebase -i c30cc --autosquash
Erfolgreich Rebase ausgeführt und refs/heads/main aktualisiert.
´´´
