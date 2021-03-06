How to run?
-----------

```bash
curl -O https://raw.githubusercontent.com/indigotech/dev-setup/master/scripts/setup.sh && env bash setup.sh
```


What does this setup install?
-----------------------------

### osx-prep.sh
  - command-line-tools

### pip.sh
  - pip

### battleschool.sh
  - Battleschool
    - XCode
    - VMWare Fusion
    - Android Studio

### homebrew.sh
  - Homebrew
    - zsh
    - wget
    - heroku-toolbelt
    - git
    - git-extras
    - mongodb
  - Homebrew Cask
    - iterm2
    - java
    - zquartz
    - sublime-text3
    - atom
    - virtualbox
    - genymotion
    - slack
    - google-chrome
    - spectacle

### rvm.sh
  - rvm
    - ruby
    - ruby gems
      - bundler
      - cocoapods
      - tqt

### nvm.sh
  - nvm
    - node

### ios-developer.sh
  - Taqtile developer keys

### oh-my-zsh.sh
  - oh-my-zsh


Manual steps
------------

### Remove scripts and battleschool folders

  1. Open Terminal or iTerm2
  2. Run `rm -rf ~/scripts ~/.battleschool`


### Add Taqtile Developer account to XCode

  1. Open XCode
  2. Open Preferences: `XCode` > `Preferences` or `⌘,`
  3. Select `Accounts` tab
  4. Add Taqtile Developer's account


### Install App Store Apps

  1. Open `App Store`
  2. Search and install the following apps
    - Sketch


### Disable Guest Account

  1. Go to `System Preferences` > `Users & Groups`
  2. Unlock the padlock on the bottom
  3. Select `Guest User` on the left
  4. Uncheck `Allow guests to log in to this computer`
  5. Uncheck `Allow guest users to connect to shared folders`
  5. Lock the padlock


### Configure iCloud

  1. Go to `System Preferences` > `iCloud`
  2. Disable all services except `Find My Mac`


Next steps
----------

  1. Oh My ZSH install script runs `env zsh` in the end. It needs to find a way to skip that or finish the zsh proccess.
  2. The script still stops in some points asking for information. Idealliy it should run unattended.
  3. App Store apps need to be installed manually. Neither Homebrew Cask or Battleschool supports that.
  4. Check if everything was installed successfully in the end and show the errors if any.
