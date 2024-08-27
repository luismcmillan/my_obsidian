[[GIT]]
```Shell
ssh-keygen -t ed25519 -C "your_email@example.com"
Your identification has been saved in /home/your_username/.ssh/id_ed25519
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
cat ~/.ssh/id_ed25519.pub # copy to github
ssh -T git@github.com #test
```