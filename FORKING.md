## WHY?

It can be a painful situation if everybody pushes code to the `master` / `main` branch. 
<br>
<hr>
<br>

## How to work?

1. Fork the repository and get it into your GitHub account. 
2. Clone your forked repository into your computer. 
3. Add references (covered later). 
4. Work in a separate branch.
5. Push the branch to your forked repository. 
6. Make a pull request for that branch.
<br>
<hr>
<br> 

## References in git

References can be thought of as places on the internet where a repository exists. You need two references to get started with. One is the conventional `origin` reference which points to your forked repository and another is a reference to the main repository of the organisation.

do:
``` bash
git remote # to check what references you have
git config --get remote.< name of reference >.url # to check what the reference points to
```

if you do not have an origin setup:
```bash
git remote add origin https://github.com/your_username/repo_name.git
```

add a reference to the main repository: 
```
git remote add upstream https://github.com/organisation_name/repo_name.git
```

*upstream* is just a conventionally accepted name. You could name it something else too.
<br>
<hr>
<br>

## Always work on your own branch, not on the `master` / `main`

```bash
# for switching to a branch that exists
git checkout < branch_name >

# for creating a new branch and switching to it as well
git checkout -b < branch_name >
```
<br>
<hr>
<br>

## Fetch periodically

There might be changes happening on the main repository. You need your local repository to be in sync with them. So keep doing the following, once/twice a day/week or whenever the project maintainers explicitly ask you to do.

```bash
git checkout main
git fetch upstream
```

This will download the latest changes from the upstream reference into your computer.
<br>
<hr>
<br>

## Pushing

```bash
git push origin < name of your branch >
```
