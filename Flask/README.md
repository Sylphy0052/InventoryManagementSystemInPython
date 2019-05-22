# Flask
## 事前準備
- Pythonのインストール
- pip
- git
- heroku

### 詳細
1. brewでインストールする．

```shell
$ brew --version
Homebrew 2.1.1
Homebrew/homebrew-core (git revision d3c0; last commit 2019-05-06)
Homebrew/homebrew-cask (git revision ef11; last commit 2019-05-06)
```

2. もしインストールされてなかったら

```shell
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

3. Homebrewのアップデート

```shell
$ brew update --force && brew upgrade
```

4. pyenvのインストール

```shell
$ brew install pyenv
$ echo 'eval "$(pyenv init -)"' >> ~/.bash_profile

$ exec $SHELL -l
```

zshの場合は，`~/.zshrc`にする

5. Python(Anaconda)のインストール

バージョン一覧の表示
```shell
$ pyenv install -l | grep anaconda
```

```shell
$ pyenv install anaconda3-5.3.1
$ pyenv global anaconda3-5.3.1
```

6. 確認
```shell
$ python --version
```

7. pyenvでPythonのバージョンの切り替え
```shell
# pyenvでインストールしたpythonのバージョンを確認
$ pyenv versions
# バージョン切り替え
$ pyenv global anaconda3-5.3.1
# インストール可能なpythonバージョン一覧を表示
$ pyenv install -l
# 指定したバージョンのインストール
$ pyenv install anaconda3-5.3.1
```

## 参考
- [study-flask](https://study-flask.readthedocs.io/ja/latest/index.html)
- [AnacondaでPython環境をインストールする](https://qiita.com/t2y/items/2a3eb58103e85d8064b6)
