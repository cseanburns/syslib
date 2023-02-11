# Setup Git and GitHub

## Setup GitHub

On GitHub.com:

1. Setup github account
1. Make email address private (optional)
	- go to Settings -> Emails
	- choose **Keep my email address private**, if you want
1. Create ssh key on your Linux server
	- add pub key to GitHub
	- go to Settings **SSH and GPG keys**
	- click on **New SSH key**
	- paste pub key from **~/.ssh/id_ed25519.pub**

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

## Use git on remote server

1. Make new directory in your home directory
1. Clone repo

	``git clone git@github.com:cseanburns/syslib.git``

1. Add or modify files in cloned repo
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
