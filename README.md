
# Git Workflow

This section outlines the Git workflow for managing feature, release, and main branches using the following Git commands.
![Screenshot (18)](https://github.com/user-attachments/assets/338cc7dc-9990-4c61-b055-cf6959af5522)

## 1. Create and work on a new feature branch

This command creates a new branch called feature and switches to it.

```bash
git switch -c feature
```

This command records changes to the repository.

```bash
git commit -m "Add new feature"
```

Another commit to record additional changes that have been made since the previous commit.

```bash
git commit -m "Update feature"
```

## 2. Switch to the main branch

Once the feature is complete and committed, This command switches your working directory back to the main branch.

```bash
git checkout main
```

If there are any changes or updates to be made to the main branch, this commit will record those changes.

```bash
git commit -m "Update main"
```

## 3. Create and work on a release branch

 This command creates a new branch called release and switches to it. The release branch is typically used to prepare for a new production release.

```bash
git switch -c release
```

After making necessary changes to the release branch, this command commits those changes.

```bash
git commit -m "Prepare for release"
```

## 4. Switch back to the main branch

This command switches back to the main branch from the release branch.

```bash
git checkout main
```

This commits changes to the main branch after switching back

```bash
git commit -m "Final commit before release"
```

## 5. Merge the feature branch into the release branch

This switches your working directory to the release branch

```bash
git checkout release
git merge feature
```

## 6. Final merge into main

After testing the release, switch back to the main branch and merge the release branch into it:

```bash
git checkout main

This merges the release branch back into the main branch, incorporating all the changes that have been tested and finalized.

git merge release
```

---

# Git Workflow with Pull Requests

This section outlines the process of creating a rule, approving a merge pull request, and merging the pull request in GitHub using screenshots to illustrate each step.

## 1. **Create Rule**

In this step, you create a rule for your project. Below is a screenshot showing the created rule:

![Screenshot (22)](https://github.com/user-attachments/assets/8108bd61-4f1e-496f-b43f-43b3c929ea72)


## 2. **Pull Request Approval**

After creating a pull request, it needs to be approved . Below is a screenshot showing the pull request approval process:

![Screenshot (23)](https://github.com/user-attachments/assets/2c900fa3-7f35-4ef6-a5b5-c684cd0e3ac5)


## 3. **After Merging the Pull Request**

Once the pull request is approved, the changes are merged into the main branch. Below is a screenshot showing the repository after the pull request has been successfully merged:

![Screenshot (24)](https://github.com/user-attachments/assets/b46b2413-2a2f-4004-8545-a7a1882599e1)


