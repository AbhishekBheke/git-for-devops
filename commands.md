
# Git Practice Commands

## Step 1: Create a Directory and Initialize a Git Repository

```bash
mkdir git-for-devops
cd git-for-devops
git init
```

- **Explanation**: 
   - `mkdir git-for-devops`: Creates a new directory called "git-for-devops."
   - `cd git-for-devops`: Moves into that directory.
   - `git init`: Initializes an empty Git repository to start tracking project files.
   
   **Use case**: This is how you start a new project that you want to manage with Git.

---

## Step 2: Create Files and Check Repository Status

```bash
touch nibba.txt nibbi.txt
git status
```

- **Explanation**:
   - `touch nibba.txt nibbi.txt`: Creates two empty files named "nibba.txt" and "nibbi.txt."
   - `git status`: Checks the current status of the repository (it will show that the two files are untracked).
   
   **Use case**: Helps you create files and see what changes are happening in your project.

---

## Step 3: Stage and Commit Files

```bash
git add nibbi.txt
git add nibba.txt
git status
git commit -m "adding nibba and nibbi"
```

- **Explanation**:
   - `git add nibbi.txt nibba.txt`: Adds both files to the staging area, which means they’re ready to be committed.
   - `git status`: Again checks the status to ensure files are ready for commit.
   - `git commit -m "adding nibba and nibbi"`: Commits the staged files to the repository with a descriptive message.
   
   **Use case**: Adds your changes to the version history, which you can track and revert back to if needed.

---

## Step 4: Deleting and Restoring a File

```bash
rm nibbi.txt
git status
git restore nibbi.txt
```

- **Explanation**:
   - `rm nibbi.txt`: Deletes the file "nibbi.txt" from your local directory.
   - `git status`: Shows that the file has been deleted.
   - `git restore nibbi.txt`: Recovers the file "nibbi.txt" back from the last commit.
   
   **Use case**: Helps you manage file deletions and recover files when needed.

---

## Step 5: Configure Git (One-Time Setup)

```bash
git config --global user.name "AbhishekBheke"
git config --global user.email "Abhishek.bheke@gmail.com"
```

- **Explanation**:
   - These commands set your GitHub username and email address globally for any repository you work on.
   
   **Use case**: Necessary for associating commits with your GitHub account.

---

## Step 6: Modify a File and Commit Changes

```bash
vim nibba.txt
git add nibba.txt
git commit -m "added changes in nibba.txt"
```

- **Explanation**:
   - `vim nibba.txt`: Opens "nibba.txt" in the Vim editor to modify its content.
   - `git add nibba.txt`: Stages the modified file.
   - `git commit -m "added changes in nibba.txt"`: Commits the changes with a message describing the update.
   
   **Use case**: Allows you to make changes and track updates in your project.

---

## Step 7: Create a New Branch and Work on It

```bash
git checkout -b dev
touch nibbu.txt
git add nibbu.txt
git commit -m "added nibbu.txt"
```

- **Explanation**:
   - `git checkout -b dev`: Creates and switches to a new branch called "dev."
   - `touch nibbu.txt`: Creates a new file named "nibbu.txt."
   - `git add nibbu.txt`: Stages the new file.
   - `git commit -m "added nibbu.txt"`: Commits the new file with a message.
   
   **Use case**: Working in branches allows you to keep new features or experiments separate from your main project until they’re ready.

---

## Step 8: Switch Between Branches

```bash
git checkout master
git log
git checkout dev
git log
```

- **Explanation**:
   - `git checkout master`: Switches back to the "master" branch.
   - `git log`: Views the commit history.
   - `git checkout dev`: Switches back to the "dev" branch.
   - `git log`: Views the commit history of the "dev" branch.
   
   **Use case**: Allows you to switch between different lines of work (branches) and keep track of separate changes.
