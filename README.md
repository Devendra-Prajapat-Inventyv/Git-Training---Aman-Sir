
# Git Workflow

This section outlines the Git workflow for managing feature, release, and main branches using the following Git commands.
![Screenshot (18)](https://github.com/user-attachments/assets/338cc7dc-9990-4c61-b055-cf6959af5522)

## 1. Create and work on a new feature branch

Start by creating a new branch for your feature:

```bash
git switch -c feature
```

Make changes to your code and commit them:

```bash
git commit -m "Add new feature"
```

Repeat the commit step if needed for additional changes:

```bash
git commit -m "Update feature"
```

## 2. Switch to the main branch

Once the feature is complete and committed, switch back to the main branch:

```bash
git checkout main
```

Commit any necessary changes on the main branch:

```bash
git commit -m "Update main"
```

## 3. Create and work on a release branch

Create a new release branch to prepare for the release:

```bash
git switch -c release
```

Commit any necessary changes to the release branch:

```bash
git commit -m "Prepare for release"
```

## 4. Switch back to the main branch

After preparing the release, switch back to the main branch:

```bash
git checkout main
```

Commit any necessary changes:

```bash
git commit -m "Final commit before release"
```

## 5. Merge the feature branch into the release branch

Switch to the release branch and merge the feature branch into it:

```bash
git checkout release
git merge feature
```

## 6. Final merge into main

After testing the release, switch back to the main branch and merge the release branch into it:

```bash
git checkout main
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


