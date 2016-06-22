# 初めてのSass

## Sass(.scss)を使う準備

### node.jsの準備（Windows編)
1.[公式サイト](https://github.com/marcelklehr/nodist)から「nodist」のインストーラーをダウンロードする  
2.インストールする  
3.コマンドプロンプトを立ち上げて、インストール可能なバージョンを確認する
```
> nodist dist
```
4.利用するバージョンのnode.jsをインストールする
```
> nodist + v4.4.5
```
5.システム全体で利用するnode.jsを設定する
```
> nodist 4.4.5
```
6.設定できたか確認する
```
> node -v
```
7.ヘルプ表示
```
> nodist --help
```

### node.jsの準備（Mac編)
1.ターミナルを起動する  
2.Githubから「anyenv」をクローンする
```
$ git clone https://github.com/riywo/anyenv ~/.anyenv
```
3.エディタで「.bash_profile」を開く（ない場合はユーザーの直下に新規作成する）  
4.下記を「.bash_profile」にコピペする
```
export PATH=$HOME/.anyenv/bin:$PATH
eval "$(anyenv init -)"
```
5.パスを有効化する
```
$ source ~/.bash_profile
```
6.必要な環境をインストールする
```
$ anyenv install ndenv
```
7.インストール可能なnode.jsのバージョンを表示する
```
$ ndenv install -l
```
8.利用するバージョンのnode.jsをインストールする
```
$ ndenv install v4.4.5
```
9.インストールされたか確認する
```
$ ndenv versions
```
10.システム全体で利用するnode.jsを設定する
```
$ ndenv global v4.4.5
```
11.設定できたか確認する
```
$ node -v
```

### Sass(.scss)を使う準備 - gulp

#### 「gulp」？
- タスクランナー（正確にはストリーミング・ビルド・システム）
- 作業を自動化してくれるツール
    - 毎回同じことを繰り返し行うような場合に便利

#### 「npm」？
- 「node package manager」
- node.jsを利用するツール群を一元管理できるもの
- node.jsのインストール時に一緒にインストールされる
```
$ npm -v
```
- npm のヘルプ表示
```
$ npm help
```

#### 読んでおくと幸せになれるかもしれない記事
- [gulp.js を今一度キチンと！gulp.js 導入基礎](https://h2ham.net/gulp-basic)

## USAGE

```
$ cd path/to/gulp/file/directory
$ npm i (if you run first time)
$ npm start
```
