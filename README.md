# developer.ottemo.io


### Clone repo and setup locally

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
hugo server
```

Then browse to your [localhost](http://127.0.0.1:1313)

## Deploy to Firebase

### configure firebase connection

```
# install firebase tools
npm install -g firebase-tools

# authenticate to firebase using your ottemo creds
firebase login
```

### push local changes to firebase

Only do this if your PR is accepted and reviewed, please. This command pushes your changes to production.

```
hugo && firebase deploy
```
