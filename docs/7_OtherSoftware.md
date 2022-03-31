<!--

This document is written in Markdown.
You can preview on such as VisualStudio Code.
If you want to know more, search with "vscode markdown" or refer to official document https://code.visualstudio.com/Docs/languages/markdown .

-->

# 7. その他のソフトのインストール

## gnuplot

グラフ作成ソフトgnuplot

aptでインストール
```
sudo apt install gnuplot
```

起動は
```
gnuplot
```

## VSCode
Microsoftのエディター

Visual Studio Codeは`VSCode`と呼ぶことVisual Studioとは別です。混ざるので`VSCode`と呼ぶように

`apt`にはないのでホームページからインストーラ(拡張子:.dpkg)を取ってくる。

[code.visualstudio.com](https://code.visualstudio.com/)

Linux x64の`.deb`を取ってくる。(stableは安定版/Insiderは更新が頻繁に行われる。 好きに選べばよい。)
Linuxにもいろいろな種類があるがUbuntuは`Debian系`という流派に属する。


ブラウザの初期設定ではDownloadsにダウンロードされるだろう。

```
_YOUR_NAME_@_MACHINE_:~$ cd Downloads
_YOUR_NAME_@_MACHINE_:~/Downloads$ ls
```
これでダウンロードしたものがわかるはずである。
インストールには`dpkg`コマンドで

```
_YOUR_NAME_@_MACHINE_:~/Downloads$ sudo dpkg -i _VSCODE_FILE_NAME_
```
とすればインストールできる。

```
code [file]
```
で起動

エディターといえば`Atom`や`Notepad++`などさまざまなものがあるが今日日`VSCode`一択である。
基本的にテキストを編集できればなんでもいい。


## Slack

サイトから.debアプリをダウンロードする。

[slack.com](https://slack.com/intl/ja-jp/downloads/linux)

同様に`.deb`がダウンロードできるので

```
sudo dpkg -i _SLACK_FILE_NAME_
```


## Edge
標準のFirefoxも悪くないが
Microsoftを信仰するしかない。

サイトにも書かれている。

[Microsoft Edge Insider Channels](https://www.microsoftedgeinsider.com/ja-jp/download/)

コピペで構わない。
```
## Setup
curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg

sudo install -o root -g root -m 644 microsoft.gpg /usr/share/keyrings/

sudo sh -c 'echo "deb [arch=amd64 signed-by=/usr/share/keyrings/microsoft.gpg] https://packages.microsoft.com/repos/edge stable main" > /etc/apt/sources.list.d/microsoft-edge-beta.list'

sudo rm microsoft.gpg

## Install
sudo apt update
sudo apt install microsoft-edge-beta
```
内容としてはaptで管理するパッケージにEdgeを追加している。

Chromeはここでは取り上げません。

----

[次のセクション "8. Secure Shell" へ](./8_SecureShell.md)

----
[Back to Home](../readme.md)

<!-- Written by Croyfet in 2022-->
