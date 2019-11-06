# STEP #1 - Create a github repo and clone it to local folder

## Log into github and create a new repo

1. Log into github
2. Go to [New Repositories](https://github.com/new)
3. On the **Create a new repository** page:
    * Enter a Repository Name
    * Enter a Description (or leave it blank)
    * Chose Public or Private
    * Check the `Initialize with README`
    * Leave `.gitinore` as `None`
    * Pick a license or leave it as None
    * Click `Create repository`
4. From the new repo's main (<> Code) page
    * Click `Clone or download`
    * and then click the save to clipboard button


## Clone the repo to a local folder

1. Open a terminal (iTerm2) window

2. Create a projects folder in your home folder.
This folder will contain the projects you are working on.
```
mkdir projects
```

3. Change to the projects folder:
```
cd projects
```

4. Clone the repo into its own folder:
You should still have the repo's url in the clipboard so it is just
`git clone ` and paste the repo's url.

It should be something like:
```
git clone git@github.com:<< YOUR_NAME >>/<< YOUR REPO'S NAME >>
```
for me it was:
```
git clone git@github.com:JamieCzuy/my_django_project.git
```

Output should be something like:
```
Cloning into 'my_django_project'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
```

5. Change to the repo's folder...
For me it was:
```
cd my_django_project
```

6. The only file in this folder should be a README:
```
ls
```

Output should be:
```
README.md
```

7. Use `git` to check the local repo status:
```
git status
```

Output should be something like:
```
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
```


7. Use `git` to check the local repo's logs:
```
git log
```

Output should be something like:
```
commit << COMMIT_ID: UUID >> (HEAD -> master, origin/master, origin/HEAD)
Author: << YOUR_NAME >> < << YOUR_GITHUB_EMAIL >> >
Date:   Wed Nov 6 14:53:32 2019 -0500

    Initial commit
```

For me it was:
```
commit 8b9b1f0bfdd9cf06a158b78a2e676a5403d1c142 (HEAD -> master, origin/master, origin/HEAD)
Author: Jamie Czuy <JamieCzuy@users.noreply.github.com>
Date:   Wed Nov 6 14:53:32 2019 -0500

    Initial commit
```
