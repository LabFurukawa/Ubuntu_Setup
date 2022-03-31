<!--

This document is written in Markdown.
You can preview on such as VisualStudio Code.
If you want to know more, search with "vscode markdown" or refer to official document https://code.visualstudio.com/Docs/languages/markdown .

-->

# 9. おわりに


## 写すな

これから様々なパッケージやソフトをインストールして使うようになるだろうが
きっとWebサイトにはそのインストール手順などが細かく記載されているだろう。
しかし手順通りでは実行しているディレクトリが違うことや、バージョンによってそのディレクトリやファイル名が変わっていたりすることは多々ある。
ネット上に載っているコマンドをコピペするだけでなく、何のコマンドを使っているのか、何のオプションが使われているのか、何のファイルを編集しているのかしっかりと確認しながらLinuxと触れあっていきたい。

## Ubuntu Server

今回のセットアップではUbuntu Desktopを使ってきたが先に記した通り、あくまでGUIやデスクトップはおまけであり、甘えである。
主目的である科学計算やサービスを運用する上でデスクトップがエラーを起こしたばかりに全システムが停止してしまうというのは望ましいことではない。
また画面の出力という行為は単純に考えると1920x1080のピクセルを例えば30fpsで書き換えるという行為である。そのための計算量やメモリ資源が無駄であるとしかいえない。
それにプログラマーサイドから見ればクリックして"ボタンが押された表示"がされたからと言って本当にその変更が適応されている保障などどこにあるだろうか。
もし本当にGUIが不要であるというならばUbuntu DesktopでなくUbuntu ServerというGUIが入っていないバージョンを使うという選択肢も考えるようになりたい。
ちなみにUbuntu ServerからUbuntu Desktopに変更したければ"sudo apt install ubuntu-desktop-minimal"で可能である。

----
[Back to Home](../readme.md)

<!-- Written by Croyfet in 2022-->
