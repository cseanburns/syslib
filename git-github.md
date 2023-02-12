# Setup Git and GitHub

## Setup GitHub

On GitHub.com:

1. Setup GitHub account
1. Make email address private (optional)
	- go to Settings -> Emails
	- choose **Keep my email address private**, if you want
1. Create ssh key on your Linux server

	`ssh-keygen -t ed25519 -C "your_email@example.com"`

1. Add ssh pub key to GitHub. To add pub key to GitHub.
	- On GitHub, go to Settings **SSH and GPG keys**
	- click on **New SSH key**
	- On server, use ``nano`` to open the file: **~/.ssh/id_ed25519.pub**.
	- Copy contents (mouse should work).
	- Paste contents into the **New SSH key** text box on GitHub.

Read more **GitHub** documentation here:

- [https://docs.github.com/en](https://docs.github.com/en)
- [How to create ssh key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

## Setup Git

Configure ``git`` on your remote server.

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

### Editing on GitHub

If you edit a file on GitHub,
to sync to your local repo on your server,
run the following command:

```
git pull origin main
```

## Markdown

Visit **Markdown** documentation here:

- [Markdown Documentation](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [Markdown Cheatsheet](https://www.markdownguide.org/cheat-sheet/)

It's okay to only know Markdown basics.
The whole point of Markdown is to
simply writing text that can be
converted to other formats,
like HTML, PDF, DOCX, ODT, etc.
