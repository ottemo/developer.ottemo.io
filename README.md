# developer.ottemo.io


### to clone repo and setup locally

```bash
# install hugo
brew install hugo

# clone the repo
git clone git@github.com:ottemo/developer.ottemo.io

# intialize and download the themes and plugins
git submodule update --init --recursive    # to init and grab all submodules

# to update the themes or plugins later use
git submodule update --recursive
```

### Run the local development server

```bash
# run with the current theme chosen
hugo serve --theme=docdock
```
