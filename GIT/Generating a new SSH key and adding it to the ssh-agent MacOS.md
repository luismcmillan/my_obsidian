[[GIT]]
```Shell
ssh-keygen -t ed25519 -C "mcmillan.luis@googlemail.com"
eval "$(ssh-agent -s)"
nano ~/.ssh/config

Host github.com
  AddKeysToAgent yes
  UseKeychain yes  
  IdentifyFile ~/.ssh/id_ed25519
ssh-add --apple-use-keychain ~/.ssh/id_ed25519
open ~/.ssh/ #Copy public key to github.com
```