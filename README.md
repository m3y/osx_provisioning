# OSX プロビジョニング

## 概要
ansible + homebrew で、osx上で利用するソフトウェアを管理する

## ansible インストール方法
```
$ sudo xcodebuild -license
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew doctor && brew update
$ brew install ansible
```

## 反映方法
```
$ ansible-playbook -i hosts -vv osx_base.yml
```

## brew 管理外アプリケーション
- memo
- rustup
- docker for mac
- appcleaner
- caffeine
- google-chrome
- google-japanese-ime
- iterm2
- karabiner-elements
- skitch
- wireshark
- Intellij-CE
- evernote
- dropbox
