# What is 1st-commits?
Getting used to developer's behavior in CYDAS.

# Getting Started
1. Install these as local. - Git Command, GitHub Desktop, VS Code
1. Clone repo from remote to local.
1. Create Branch, change to Pull Request, Request Review and Merge it to Master branch.

# ワークフローマニュアル

### __1.リモートリポジトリをローカルにコピーする__
1. https://github.com/CYDASCOM/リポジトリ名 にアクセスする。
1. 画面中央ペイン右上のボタン「↓Code▼」から「Open with Github Desktop」を選択する。
1. Github Desktopが起動するので、ローカルのclone先を確認しリポジトリのcloneを実行する。
1. 実行後、Github Desktop画面にてGithub(web)と同じファイルがあることを確認できる。
1. VS Code を起動し、リポジトリをcloneしたディレクトリを開く。

### __2.ブランチの作成と統合__
1. VS Code 画面左下ブランチ名称クリック「＋新しい分岐の作成」を選択する。
1. ブランチ名称を入力し作成する。(作成後画面左下のブランチ名称を確認すると作成した名称に切り替わる)
1. 作成したブランチの中でファイルを編集し保存する。
1. 保存後、左タブの「ソース管理」を開く。
1. 変更に出てきたファイルを確認する。
1. 内容が問題ない場合は、変更上の入力欄にコミットメッセージを記載してコミットする。

### __3.プッシュしよう（Push）__

1. GitHub Desktop の `Publish Branch` または `Push origin`ボタンをクリック
  * `Current Branch` のブランチが `Current Repository` に対してPushされる
  * `Current Branch` がまだ一度もPushされていない場合は `Publish Branch` それ以外の場合は `Push origin` が表示される

### __4.プルしよう（Pull）__
1. VS Code 画面左下ブランチ名称クリックし、リモートブランチを選択する。
1. 画面左サイドバーのソース管理アイコンをクリックする。
1. ソース管理パネル上部にある「…」から「プル」を選択する。
1. ローカルブランチにリモートブランチの変更が反映される。

### __5.コンフリクトが起きたときの対処法__
1. コンフリクトを解除する。
1. ファイルを編集して保存する。
1. Description箱に編集内容を記入する（例：Merge conflict)。
1. コミットボタンを押す。
1. 再プッシュする。

### __6.プルリクエストからマージまでの流れ__


### __7.不要になったリモートブランチを削除する__
1. マージ後、「Delete branch」が表示されるのでクリックしてbranchを削除する。
1. "deleted the［branch名］branch now" とメッセージが出たら削除の完了。

### __8.不要になったローカルブランチを削除する__
1. VS Code 画面左下ブランチ名称をクリックし、削除対象のブランチとは別のブランチを選択しておく。
1. ターミナル画面で　git branch -d [削除したいローカルブランチ名]　を実行する。
1. Deleted branch [削除したローカルブランチ名] と返ってくれば成功
