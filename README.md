This repo is a container for demo app repositories.
Each subdirectory is a git submodule for one demo app.


Initial Setup of Top Level Project
----------------------------------

```
cd ~/source/github.com/coreinfra-org/
git clone "git@github.com:coreinfra-org/demo-apps.git"
touch README.md
gacp

git submodule add --force "git@github.com:coreinfra-org/app-base-c.git"
git submodule add "git@github.com:coreinfra-org/app-base-golang.git"
git submodule add "git@github.com:coreinfra-org/app-base-java.git"
git submodule add "git@github.com:coreinfra-org/app-base-nodejs.git"
git submodule add "git@github.com:coreinfra-org/app-base-python.git"
git submodule add "git@github.com:coreinfra-org/app-flask-auth0.git"
git submodule add "git@github.com:coreinfra-org/app-flask-authlib.git"
git submodule add "git@github.com:coreinfra-org/app-flask-bootstrap.git"
git submodule add "git@github.com:coreinfra-org/app-flask-golinks.git"
git submodule add "git@github.com:coreinfra-org/app-flask-ipaddr.git"
git submodule add "git@github.com:coreinfra-org/app-flask-multitest.git"
git submodule add "git@github.com:coreinfra-org/app-flask-openai.git"
git submodule add "git@github.com:coreinfra-org/app-flask-wiki.git"
git submodule add "git@github.com:coreinfra-org/app-hugo-site.git"
gacp

for dir in app-*/; do (cd "$dir" && touch README.md && gacp); done
gacp
```


Usage
-----

* https://stackoverflow.com/questions/12641469/list-submodules-in-a-git-repository

```
git clone "git@github.com:coreinfra-org/demo-apps.git"
cd demo-apps
git submodule init
git submodule update
git status
git submodule status
bat .gitmodules
git diff --cached --submodule
git log -p --submodule
```
