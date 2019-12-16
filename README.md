For playbook requiring ssh keys (ie anything donwloading from git)
```bash
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
```

# python.yml
installs dependencies and setups environment variables in bash_profile for pyenv. Still need to manually run the pyenv installer
```bash
curl https://pyenv.run | bash
```

# rbenv
after running the playbook, it will still be missing some setup before use
```bash
rbenv init
exec $SHELL
```
