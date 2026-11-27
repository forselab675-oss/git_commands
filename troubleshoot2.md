git remote set-url origin https://forselab675-oss@github.com/forselab675-oss/MavenWeb.git
git config --local credential.username forselab675-oss
git config --local credential.useHttpPath true
"protocol=https`nhost=github.com`npath=forselab675-oss/MavenWeb.git`nusername=gandhi09m1-dotcom`n`n" | git credential-manager erase
git push -u origin main
