# fullstack-mac

> Curated list of stuff to work on mac

- Tools
 - xCode
 - [NVM](https://github.com/creationix/nvm)
 - [Android Studio](https://developer.android.com/studio/index.html)
 - [JDK](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
 - [Ionic2](http://ionicframework.com/docs/v2/resources/platform-setup/mac-setup.html)
 - [PIP](https://pip.pypa.io/en/stable/installing/)
 - [EB](http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/eb-cli3-install.html)
 
- Apps
 - 7zX
 - Clean My Mac 3
 - Dr. Cleaner
 - [Slack](https://slack.com/downloads/osx)
 - Spotify
 - uTorrent
 - Visual Studio Code


### AWS EB CLI
```
$ sudo pip install --upgrade --user awsebcli
```

### AWS CLI
```
$ sudo pip install awscli --ignore-installed six
```

### ˜/.bash_profile

```
# Ionic Platform Permissions to load on xcode
alias ionic-perm='sudo chmod -R +x ./platforms && sudo chmod -R +x ./plugins && sudo chown -R $(whoami) ./platforms && sudo chown -R $(whoami) ./plugins && sudo chown -R $(whoami) ./src && sudo chmod -R +x ./src && sudo chown -R $(whoami) ./.tmp && sudo chmod -R +x ./.tmp'

# create a JAVA_HOME variable, determined dynamically
export JAVA_HOME=$(/usr/libexec/java_home)

# Add that to the global PATH variable
export PATH=${JAVA_HOME}/bin:$PATH

# Add the Android SDK to the PATH variable
export PATH=${PATH}:~/Library/Android/sdk/tools:~/Library/Android/sdk/platform-tools:~/Library/Android/sdk/build-tools/25.0.1

# Make ls use colors
export CLICOLOR=1
alias ls='ls -Fa'

# set nvm
export NVM_DIR="/Users/st1s/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh"  # This loads nvm

# For EB
export PATH=${PATH}:~/Library/Python/2.7/bin

# define colors
C_DEFAULT="\[\033[m\]"
C_WHITE="\[\033[1m\]"
C_BLACK="\[\033[30m\]"
C_RED="\[\033[31m\]"
C_GREEN="\[\033[32m\]"
C_YELLOW="\[\033[33m\]"
C_BLUE="\[\033[34m\]"
C_PURPLE="\[\033[35m\]"
C_CYAN="\[\033[36m\]"
C_LIGHTGRAY="\[\033[37m\]"
C_DARKGRAY="\[\033[1;30m\]"
C_LIGHTRED="\[\033[1;31m\]"
C_LIGHTGREEN="\[\033[1;32m\]"
C_LIGHTYELLOW="\[\033[1;33m\]"
C_LIGHTBLUE="\[\033[1;34m\]"
C_LIGHTPURPLE="\[\033[1;35m\]"
C_LIGHTCYAN="\[\033[1;36m\]"
C_BG_BLACK="\[\033[40m\]"
C_BG_RED="\[\033[41m\]"
C_BG_GREEN="\[\033[42m\]"
C_BG_YELLOW="\[\033[43m\]"
C_BG_BLUE="\[\033[44m\]"
C_BG_PURPLE="\[\033[45m\]"
C_BG_CYAN="\[\033[46m\]"
C_BG_LIGHTGRAY="\[\033[47m\]"

# set your prompt
export PS1="\n$C_LIGHTGREEN\u$C_LIGHTYELLOW@$C_LIGHTGREEN\h$C_YELLOW:$C_LIGHTYELLOW\w$C_LIGHTGRAY\n\$$C_DEFAULT "
```
