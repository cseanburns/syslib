# Setup Git and GitHub

## Setup GitHub

On GitHub.com:

1. Setup github account
	- go to Settings -> Emails
	- choose **Keep my email address private**, if you want
2. Click on the + sign in GitHub
	- click on New repository
3. Create ssh key
	- add pub key to GitHub
4. Clone repo

Read more **GitHub** documentation here:

[https://docs.github.com/en](https://docs.github.com/en)

## Setup Git

Configure ``git`` on your local machine.

1. Configure your identity.
From the command prompt:

```
git config --global user.name "First Name Last Name"
git config --global user.email "firstlast@example.com"
git config --global core.editor nano
git config --global init.defaultBranch main
```

2. Check your settings:

```
git config --list
```

Read more ``git`` documentation here:

[https://git-scm.com/](https://git-scm.com/)

## Use git

1. Added or modify files in your repo
2. Track changes with:
	
	```
	git add .
	```

3. Commit changes and add message with:

	```
	git commit -m "add message in quotes"
	```

4. Push changes to remote repo with:

	```
	git push origin main
	```


## Markdown

Visit **Markdown** documentation here:

https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

Only need to know the basics.
