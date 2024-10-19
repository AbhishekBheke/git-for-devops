mkdir git-for-devops          # Create a directory for the Git project
cd git-for-devops             # Navigate into the directory
clear                         # Clear the terminal screen
ls                            # List files and directories (there would be none yet)
pwd                           # Show the current directory path
git init                      # Initialize a Git repository in the current directory
clear                         # Clear the terminal screen
git status                    # Check the status of the Git repository
touch nibba.txt nibbi.txt     # Create two new empty files
git status                    # Check the status of files (new files will be untracked)
git add nibbi.txt             # Add "nibbi.txt" to the staging area
git add nibba.txt             # Add "nibba.txt" to the staging area
git status                    # Check the status to see if files are in the staging area
git commit -m "adding nibba nibbi"  # Commit the staged changes with a message
rm nibbi.txt                  # Remove "nibbi.txt"
git status                    # Check the status (file will be marked as deleted)
git restore nibbi.txt         # Restore the deleted file from the working directory
git config --global user.name "AbhishekBheke"  # Set global Git username
git config --global user.email "Abhishek.bheke@gmail.com"  # Set global Git email
git status                    # Check the status again (likely no changes)
git add nibba.txt             # Stage "nibba.txt" for commit
git status                    # Check the status
git commit -m "This is checking"  # Commit changes with a message
git log                       # View the commit history
vim nibba.txt                 # Open "nibba.txt" in the Vim editor to modify it
git add nibba.txt             # Stage the modified file for commit
git commit -m "added changes in nibba.txt"  # Commit the changes with a message
git log                       # View the commit history
clear                         # Clear the terminal screen
git checkout -b dev           # Create and switch to a new branch named "dev"
touch nibbu.txt               # Create a new file "nibbu.txt"
git status                    # Check the status of the new file
git add nibbu.txt             # Stage "nibbu.txt" for commit
git commit -m "added nibbu.txt"  # Commit the new file with a message
git checkout master           # Switch back to the "master" branch
git log                       # View the commit history on "master"
git checkout dev              # Switch back to the "dev" branch
git log                       # View the commit history on "dev"
