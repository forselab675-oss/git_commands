1. Check remote URL
git remote -v


2. Set correct remote URL
git remote set-url origin https://forselab675-oss@github.com/forselab675-oss/git_commands.git


Ensures Git pushes to the correct repository.

3. Set repository-specific username
git config --local credential.username forselab675-oss
git config --local credential.useHttpPath true


Configures credentials for this repository only.

4. Check credential helper
git config --show-origin --get-all credential.helper


5. Clear only this repository's cached credential (PowerShell)
"protocol=https`nhost=github.com`npath=forselab675-oss/git_commands.git`nusername=gandhi09m1-dotcom`n`n" | git credential-manager erase


Clears the cached credential for this repository, not other projects.

6. Push again
git push -u origin abc


Replace abc with your branch name and authenticate with an account that has write access.
