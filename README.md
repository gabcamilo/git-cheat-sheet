# Git Cheat Sheet

## git config
`git config --local`
`git config --global`
`git config --system`

`git config --global core.editor code`

`git config --global --edit`

### Personal .gitconfig
```
[core]
	editor = code --wait
[user]
	email = theemail@mail.com
	name = Jane Doe
[push]
	followTags = true
[alias]
	c = !git add --all && git commit -m
	s = !git status -s
	l = !git log --pretty=format:'%C(blue)%h%C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'
	amend = !git add --all && git commit --amend --no-edit
	count = !git shortlog -s --grep
```

## git log
logs the past commits

## git status
`git status -s` (short version)

## git tag
`git tag "personal-tag"`

`git tag -a "1.0.1" -m "1.0.1"` (to mark releases)
