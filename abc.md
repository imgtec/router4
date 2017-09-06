## ubntu 16.04 ##

```
# 2016.4.25
  sudo apt-get autoremove -y nano 
# Install packages on ubuntu 16.04

sudo apt-get -y install gcc-multilib

# base system
  sudo apt-get -y install vim
# sudo apt-get -y install emacs24-nox 
  sudo apt-get -y install tree
  sudo apt-get -y install tmux
  sudo apt-get -y install bc
# sudo apt-get -y  install irssi
# sudo apt-get -y install screen
# sudo apt-get -y install gawk
# sudo apt-get -y install nautilus-open-terminal
  sudo apt-get -y install lrzsz
# sudo apt-get -y install unzip
# sudo apt-get -y install zip
  sudo apt-get -y install p7zip-full

# base dev
  sudo apt-get -y install make
  sudo apt-get -y install git
# sudo apt-get -y install git-email 
  sudo apt-get -y install mutt
# sudo apt-get -y install g++
# sudo apt-get -y install gcc
# sudo apt-get -y install build-essential


# u-boot, bare programs
# sudo apt-get -y install tftpd-hpa
  sudo apt-get -y install ckermit
# sudo apt-get -y install minicom

# networking 
# sudo apt-get -y install vtun
# sudo apt-get -y install vlan
# sudo apt-get -y install bridge-utils
# sudo apt-get -y install pptp-linux
# sudo apt-get -y install autossh 
# sudo apt-get -y install traceroute
# sudo apt-get -y install ddclient

# servers
# sudo apt-get -y install samba
# sudo apt-get -y install nfs-kernel-server
# sudo apt-get -y install inetutils-ftpd

# Android
# sudo apt-get -y install build-essential
# sudo apt-get -y install gperf
# sudo apt-get -y install lib32stdc++6
# sudo apt-get -y install libstdc++6
# sudo apt-get -y install flex
# sudo apt-get -y install gperf

# linux kernel
# sudo apt-get -y install exuberant-ctags
  sudo apt-get -y install libncurses-dev
  sudo apt-get -y install u-boot-tools
  sudo apt-get -y install lzop

# sudo apt-get -y install zlib1g-dev
# sudo apt-get -y install libtool
# sudo apt-get -y install automake
# sudo apt-get -y install libusb-1.0-0-dev
# rtems
# sudo apt-get -y install bison g++ flex texinfo unzip zlib1g-dev python-dev
```


## TMUX ##
全局配置文件`/etc/tmux.conf`

```
set-option -g prefix C-Space
unbind-key C-b
bind-key C-Space send-prefix

bind-key Space last-pane
bind-key C-Space  last-window

bind-key C-n next-window
bind-key C-p previous-window

bind-key C-w set-window-option force-width 80

set-window-option  -g mode-keys vi

set -g history-limit 4096
```
