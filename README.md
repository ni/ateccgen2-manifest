# Prerequisite #

### Repo and Git ###
Install the repo bootstrap binary:
```
$  mkdir ~/bin
$  export PATH=~/bin:$PATH
$  curl https://commondatastorage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
$  chmod a+x ~/bin/repo
```
Alternatively, in Ubuntu, repo may be installed as part of the `phablet-tools` package.

Install Git and configure user name and e-mail. Below is an example for Debian-based systems:
```
$ sudo apt install git
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```

# Building RCU Image #
Create a directory for your OE-Core setup to live in and clone the meta-information:
```
$ mkdir ${HOME}/oe-core
$ cd ${HOME}/oe-core
$ repo init -u https://github.com/ni/smartracks-manifest.git -b $GITBRANCH -m smartracks-manifest.xml
$ repo sync
```
Replace $GITBRANCH with the branch name that you would like to sync the manifest from, e.g. `main`

Source the file export to setup the environment:
```
$ . export
```

Build the image:
```
$ bitbake smartracks-minimal-image
```
