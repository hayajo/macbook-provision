# Macの開発環境構築

## 初期構築

### Xcodeをインストール

Mac App StoreからXcodeをインストール。

その後、ターミナルから下記コマンドを実行してライセンスに同意し、Command Line Toolのインストールを行う。

    sudo xcodebuild -license
    xcode-select --install

### Homebrewをインストール

    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    brew doctor
    brew update

### Pythonをインストール

    brew install python

### Ansibleをインストール

    pip install ansible

### Ansibleでアプリケーションをインストール

    ansible-playbook -i hosts -vv localhost.yml

## 更新

アプリケーションの更新ではAnsibleのみ実行する。

    ansible-playbook -i hosts -vv localhost.yml

## ghq

    export GOPATH=$HOME
    export PATH=$GOPATH/bin:$PATH
    go get github.com/motemen/ghq

## VirtualBox, Vagrant, Chrome

* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* [Vagrant](https://www.vagrantup.com/downloads.html)
* [Chrome](https://www.google.co.jp/chrome/browser/desktop/index.html)

