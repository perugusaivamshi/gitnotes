🟢 GIT CONFIGURATION (one-time setup)
Command                                                  	Use
git config --global user.name "Your Name"               	Set your Git username
git config --global user.email "your.email@example.com"	  Set your Git email
git config --global init.defaultBranch main	              Set default branch to main
git config --global credential.helper store	              Save GitHub credentials permanently

📂 REPO MANAGEMENT
Command	                                                  Use
git init	                                Initialize a new Git repository
git clone <repo-url>	                    Clone an existing repo
git remote -v                            	View remote URL(s)
git remote set-url origin <new-url>	      Change remote URL (e.g. from HTTPS to SSH)

📄 STAGING & COMMITTING CHANGES
Command                              	Use
git status	                         Show current file status
git add <file>	                     Stage a specific file
git add .	                           Stage all changes in current directory
git commit -m "Your message"	       Commit staged changes
git restore <file>	                 Undo changes in working directory (before staging)
git reset <file>	                   Unstage a file

🌍 BRANCHING
Command                         	Use
git branch	                         List branches
git branch <name>	                   Create a new branch
git checkout <name>                  Switch to a branch
git checkout -b <name>               Create and switch to a new branch
git merge <branch>	                  Merge a branch into current one
git branch -d <name>	                Delete a branch locally

🔄 PUSH & PULL (REMOTE WORK)
Command	                         Use
git push origin <branch>	      Push local commits to remote
git pull origin <branch>	      Pull changes from remote repo
git fetch	                      Fetch latest changes (doesn’t merge)

🕵️‍♂️ VIEWING HISTORY
Command	                         Use
git log	                         View commit history
git log --oneline	               Short log format
git show <commit-id>	           Show details of a specific commit
git diff	                       See unstaged changes
git diff --staged	               See staged changes

🔁 UNDOING & RESETTING
Command                         	Use
git revert <commit-id>	         Undo a commit by making a new one
git reset --hard <commit-id>	   Reset to a previous commit (⚠️ destructive)
git clean -fd	                   Delete untracked files/directories

🔄 WORKING WITH TAGS
Command	              Use
git tag	              List tags
git tag <name>	      Create a new tag
git push origin <tag>	Push a specific tag
git push origin --tags	Push all tags

🔐 SSH AUTHENTICATION (Bonus)
Command                                                  	Use
ssh-keygen -t ed25519 -C "your.email@example.com"	        Generate SSH key
eval "$(ssh-agent -s)"                         	          Start SSH agent
ssh-add ~/.ssh/id_ed25519	                                Add key to agent
cat ~/.ssh/id_ed25519.pub	                                Show public key (add this to GitHub)

🧹 EXTRAS
Command                           	Use
git stash	                          Temporarily save changes you don’t want to commit yet
git stash pop	                      Reapply stashed changes
git cherry-pick <commit-id>	        Apply a specific commit from another branch
git reflog	                        Show all history of HEAD (good for recovering lost work)
