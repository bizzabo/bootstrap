Bootstrap
=========

## Motivation

Setting up a new developer machine can be an **ad-hoc, manual, and time-consuming** process.  `bootstrap` aims to **simplify** the process with **easy-to-understand instructions** :

### But...I Don't Need All These Tools!

**`bootstrap` is geared to be more of an organized *reference* of various developer tools.**

If you're interested in automation, `bootstrap` provides a customizable [setup script](#single-setup-script).  There's really no one-size-fits-all solution for developers so you're encouraged to make tweaks to suit your needs.

### Single Setup Script

#### Running with Git

##### Clone the Repo

    $ git clone https://github.com/danieldop/bootstrap.git && cd bootstrap

##### Run scripts using command line

**Since you probably don't want to install every section**, you can just run each script separately. Below are some examples.

Run `zsh.sh`, `osxprep.sh`, `brew.sh`, and `osx.sh` - common libraries:
```bash
sh zsh.sh
sh osxprep.sh
sh brew.sh
sh osx.sh
```

Run `osxprep.sh`, `brew.sh`, and `osx.sh`, and `datastores.sh`:
```bash
sh zsh.sh
sh ops.sh
sh brew.sh
sh datastores.sh
```

Scripts geared towards Front-End engineer: 
```bash
sh zsh.sh
sh osxprep.sh
sh brew.sh
sh ops.sh
sh web.sh
```

Scripts geared towards Back-End engineer: 
```bash
sh zsh.sh
sh osxprep.sh
sh brew.sh
sh ops.sh
sh server.sh
```

Scripts geared towards Mobile engineer: 
```bash
sh zsh.sh
sh osxprep.sh
sh brew.sh
sh ops.sh
sh mobile.sh
```

#### Scripts

* [osxprep.sh](https://github.com/danieldop/bootstrap/blob/master/osxprep.sh)
    * Updates OS X and installs Xcode command line tools
* [brew.sh](https://github.com/danieldop/bootstrap/blob/master/brew.sh)
    * Installs common Homebrew formulae and apps
* [osx.sh](https://github.com/danieldop/bootstrap/blob/master/osx.sh)
    * Sets up OS X defaults geared towards developers
* [web.sh](https://github.com/danieldop/bootstrap/blob/master/web.sh)
    * Sets up JavaScript web development
* [server.sh](https://github.com/danieldop/bootstrap/blob/master/server.sh)
    * Sets up Java development
* [ops.sh](https://github.com/danieldop/bootstrap/blob/master/ops.sh)
    * Sets up K8s & Helm development
* [datastores.sh](https://github.com/danieldop/bootstrap/blob/master/datastores.sh)
    * Installs MySQL, MongoDB, Redis, ElasticSearch and DB IDEs - Sequel Pro & RoboMongo
* [mobile.sh](https://github.com/danieldop/bootstrap/blob/master/mobile.sh)
    * Installs iOS Env|Android Env|React-Native Env

**Notes:**
* Before installing mobile.sh please make sure to install Xcode from AppStore or Developer poortal first.
* When installing the Xcode command line tools, a dialog box will confirm the installation.
    * Once Xcode is installed, follow the instructions on the terminal to continue.
* `brew.sh`, which takes a while to complete as some formulae need to be installed from source.
* **When scripts complete, be sure to restart your computer for all updates to take effect.**
