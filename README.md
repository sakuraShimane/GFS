# Forked from jin/237/GFS しています。
　主に作業で参考にしたサイトを書いて行きます。

# GFS(じーふす)　by Team KOCHODANI
Information Processing Examinations Assistant Service<br>
プロジェクト内容：情報系の資格取得を支援するためのコミュニティサイトの作成を行う

# Members
- Chief Executive Officer & Project Leader::<br>__じん__(https://github.com/jin237)
- Front-end Engineer & Designer::<br>__さくら__(https://github.com/sakuraShimane)
- Back-end Engineer & Infrastructure Engineer::<br>__わたる__(https://github.com/nodoka8)
- Front-end Engineer & Back-end Engineer::<br>__もりもり__(https://github.com/OhyoriMasanobu)
- Back-end Engineer & Infrastructure Engineer::<br>__えばちゃそ__(https://github.com/ebatyaso1228)


### 現在の目標
ユーザ1000人

#### 進行状況
下記のURLにて確認<br>
https://github.com/jin237/Sea-Whale_project/projects/1


## Symbol Mark
ムササビを元にした画像の用意(作成中)

## The Service Introduction Page
- [【Main Page】](https://determined-banach-55a167.netlify.app/)
- [【src Page in Github】](https://github.com/jin237/gfs_website)


## Concept
### 質問で繋がる、発想で共有、成長で最高の状態へ
資格取得を目指すためには、知らないことを０、１から学ぶことが多い。独学では限界がある。
入門者にとって難しいことは、ある程度の知識を持つものが教えること、または教え合うことで向上精神と成長を感じることができる。
これらの繋がりによって、得られたアイデアや知識を総動員することで、新たなアイデア、サービスが生まれる。
記事、コミュニティを「気軽に」「自由に」「簡単に」探すことや発言ができるのであれば、もっともっと活発なIT業界への入門も仲間もできる。
そうして、資格取得であったり、「成長」を感じつことができる状態で、実践環境に身を置くことができる。


## Contents
- 気軽に投稿できるTwitterモデルの「__ムルムル(murmur)__」
- イベントやTL会などを貼ることができる「__インフォメーション（information）__」
- 一定のコミュニティを作ることができる「__コミュニティ(Community)__」
- プロフィール

※今後変更の可能性あり

## Frameworks, Developement Languages
### Framework
- Django(Python Framework)
- Vue.js(JavaScript Framework)

### Language
- Python
- JavaScript
- HTML/CSS

### Cloud Computing Service
- Amazon Web Service (AWS)
- Google Cloud Platform (GCP)


## KOCHODANI Developmet Members Profiles
#### じん
- 【Wix（My page）】->https://fgdaojebvoa237.wixsite.com/mysite
- 【Note】->https://note.com/jin237
- 【Twitter】->https://twitter.com/home?lang=ja
- 【Facebook】->https://www.facebook.com/takehiro.iino.3/
- 【Qiita】->https://qiita.com/jin237
#### さくら
- 【Git My Page】->https://sakurashimane.github.io/
- 【Twitter】->https://twitter.com/shimanenosakura
- 【Facebook】->https://www.facebook.com/sakura.nishikori
#### わたる
- 【Twitter】->https://twitter.com/nodonod8
- 【Portforio】->https://fori.io/WataruOmori
#### もりもり
- 【Facebook】->https://www.facebook.com/ohyori/
#### えばちゃそ
- 【Qiita】 ->https://qiita.com/ebatyaso1228

## Roadmaps
#### 画面遷移Roadmap
<img src="https://github.com/jin237/GFS/blob/main/github_readme/GFS_Roadmap.png" height=300px>

## 環境構築手順
https://daily-line-76f.notion.site/docker-compose-fb61da987ea94988a4cdaf66f7785a40  

7/14追記: docker-compose を使用した開発に変更のため下記の構築手順使用しません  
https://www.notion.so/PC-54b90da196d24d5fb01b9a5779fc230b

## Gitを使用した開発フロー
https://daily-line-76f.notion.site/Git-4f0b175fa5ff409c8cfa4e6ef8bcbd8e
### Git、GitHubに関するまとめ
https://mirror-summer-bcf.notion.site/Git-Git-Git-9a9417c1549d4a01b6dd4c0d3a88acef

## DB設計　初期バージョン 
<img src="https://user-images.githubusercontent.com/57553474/125299744-65dab980-e364-11eb-95af-1bdbc352c747.png" height=300px>


## 基本機能について
基本的な機能については以下の５つの項目で行う．
- murmur（ムルムル）
- information（インフォメーション）
- community（コミュニティ）
- profile（プロフィール）
それぞれについてのデザインの仮案と詳細機能について記述を行う．

##### tempalte（おおもと）：
__＜ヘッダー＞__
```markdown
  - アプリ名
  - 時間
  - アカウントアイコン
  - ナビゲーション
```


__＜フッター＞__
```markdown
  - プライバシーポリシー
  - マーク
  - 会社（チーム）概要
  - 機能説明
```

##### murmur（ムルムル）：
```markdown
- 投稿の本体
	- アイコン
	- ID
	- 投稿時間
- Nice（いいね）：数，色
- React（反応）：数，色
- Quote（引用）：数，色
- リプライ（投稿本体）
- 共有：リンク取得，埋め込み，報告，広告，アナリティクス，ヘルプ
```

##### community（コミュニティ）：
```markdown
- チャンネル
- チャット本体：top image, ID
- 投稿時間（送信時間）
- コミュニティ名
- コミュニティの説明
- コミュニティルール
- Nice（いいね）：数，色
- React（反応）：数，色
- Quote（引用）：数，色
- 共有：リンク取得，コード引用，埋め込み，報告，広告，アナリティクス，ヘルプ
```

##### profile（プロフィール）：
```markdown
diaryと一緒，またはこれらを簡潔にまとめたものや，murmur, scraps, communityを含めたものになる．
- top image
- ID
- 名前
- DM機能ボタン
- 投稿者についての説明
- 属しているcommunity
- murmur投稿一覧
- scraps投稿一覧
- community投稿一覧
- 設定画面ボタン
```


# windowsでのgfsの環境構築（途中から)
### pythonの導入
pythonのパッケージを[ここ](https://pythonlinks.python.jp/ja/index.html)からインストール<br>
インストールしたパッケージの.exeファイルをその場で実行<br>
そのときに出てきた画面で、

- [x] Install laucher for all users (recommended)
- [ ] Add Python 3.9 to PATH

となっているのでチェックを付ける。
そしたら、Customize installationを選択する。
全部の項目にチェックがついてることを確認して、nextボタンをぽちっ。

- [ ] Precompile standard library
にdirチェックを入れる。
この時に、ファイルの場所（C:\Users\[user_name]\AppData\Local\Programs\Python\Python39）を覚えておく。

そしたらInstallする。
おわったら、そのままClose

念のために環境変数を見てみてpathが通ってるか確認する。（たぶん通ってる）

そのままcmdお開いて、"python"を入力して、
```
Python 3.9.6 (tags/v3.9.6:db3ff76, Jun 28 2021, 15:26:21) [MSC v.1929 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>>
```
が出てくればOK
抜けたい場合、'''exit()'''を入力すれば、抜けれる。

通ってるはずだが、pipはだいたい古いのが入るのでアップグレードする。
```python
python -m pip install --upgrade pip
```

### dockerの立ち上げと、pythonでの実行まで
この後は、
```
cd Users\[user_name]\Documents\GitHub\GFS\app
C:\Users\[user_name]\Documents\GitHub\GFS\app> docker-compose up -d
C:\Users\[user_name]\Documents\GitHub\GFS\app> docker ps

C:\Users\[user_name]\Documents\GitHub\GFS\app> docker-compose exec gfs-web bash
root@026d6dcceffa:/app# cd GFSProject
root@026d6dcceffa:/app/gfsproject# python manage.py runserver 0:8000

>>>
Watching for file changes with StatReloader
Performing system checks...

<django.db.models.fields.related_descriptors.ForwardOneToOneDescriptor object at 0x7ffaee2f4310>
System check identified no issues (0 silenced).
September 03, 2021 - 16:40:05
Django version 3.2.7, using settings 'GFSProject.settings'
Starting development server at http://0:8000/
Quit the server with CONTROL-C.
```

これで完了！
この後は、[http://localhost:8000/](http://localhost:8000/) コネクト
そうすると、ＧＦＳのプロダクトの中身が見れる。

★python manage.py runserver 0:8000したあとに出る
  ModuleNotFoundError: No module named 'rest_framework'

[1]requirements.txtにこれを追記
```
Django  
mysqlclient  
djangorestframework  
django-crispy-forms  
pillow  
```
[2]この3つをインストール
```
pip3 install djangorestframework
pip3 install django-crispy-forms
pip install pillow
```

[3]とめるとき

```
Ctrl+C
exit
docker stop

```
たぶんこういうエラーいわれる
```
ModuleNotFoundError: No module named 'crispy_forms'  
ModuleNotFoundError: No module named 'PIL'
```

コマンドでリモートリポジトリのoriginをローカルリポジトリに反映させる
GFSのした…

cdコマンドで.git(隠しファイルの可能性あり)があるところまで移動

```
//リモートリポジトリのすべてのブランチの更新履歴をリモート追跡ブランチに取り込む
git fetch origin 

//リモートブランチの変更をローカルブランチに反映させる
git pull
```

//error: Your local changes to the following files would be overwritten by merge:　こんなエラー出たら
//ローカルにcommitしてないものがあるよ、上書きされちゃうよ！っていう注意
//これはcommitかmargeをすればいいが、中途半端だからcommitしたくない　なら…👇


```
git stash
```
