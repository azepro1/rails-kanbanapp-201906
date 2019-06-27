# Kanban App


## 概要
タスク管理のためのアプリ


## 環境

開発（Cloud9: /kanban/kanban）
https://dfd909104a2c4c7c964fa06d5b09a045.vfs.cloud9.us-east-2.amazonaws.com/

本番（Heroku）
https://rails-kanbanapp-201906.herokuapp.com


## コマンド

準備
```
$ cd kanban
$ rails s

$ git fetch
$ git branch -a
$ git diff remotes/origin/master
$ git pull origin master

$ git checkout -b [ブランチ名]
```

コミットとマージ
```
$ git add -A
$ git commit -am "[コミットメッセージ]"
$ git status
$ git checkout master
$ git merge [ブランチ名]
```

リモートレポジトリへのpush
```
$ git remote -v
$ git push origin master
$ git push heroku master
$ heroku pg:reset DATABASE
$ heroku run rails db:migrate
$ heroku run rails db:seed
```
