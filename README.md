# Macbook Development Environment Provision

## Preparation

### Install Xcode Command Line Tools

Before installing Xcode Command Line Tools, we neeed to agree its license.

    sudo xcodebuild -license
    xcode-select --install

### Install Homebrew

    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    brew doctor
    brew update

### Install Python

    brew install python3
    pip3 install --upgrade pip setuptools

### Install Ansible

    pip3 install ansible

## Apply the playbook to install everything

    ansible-playbook -i localhost, -vv playbook.yml

## Update

    ansible-playbook -i localhost, -vv playbook.yml

## Install ghq

[motemen/ghq: Remote repository management made easy](https://github.com/motemen/ghq)

    export GOPATH=$HOME
    export PATH=$GOPATH/bin:$PATH
    go get github.com/motemen/ghq

## Install VirtualBox, Vagrant, Chrome, Docker

* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* [Vagrant](https://www.vagrantup.com/downloads.html)
* [Chrome](https://www.google.co.jp/chrome/browser/desktop/index.html)


## Intall Docker

[Docker Toolbox](https://www.docker.com/products/docker-toolbox) or [Docker for Mac](http://www.docker.com/products/docker#/mac)

## Thanks

* @soulmachine

