scala
=====



# 導入手順
- 環境：macOSX
- 前提：Java環境導入済み

## Scalaインストール
### ダウンロード
- まず、下記公式HPからアーカイブ版を取得し、展開。
- http://www.scala-lang.org/download/

### パス通す
上でダウンロードしたものを展開し、管理しやすくするためフォルダを移動。

```
$ mv ~/Downloads/scala-2.11.4 /usr/local/share/
```

`~/.bash_profile`にパス記述。

```
$ vim ~/.bash_profile

export SCALA_HOME=/usr/local/share/scala-2.11.4
export PATH=$PATH:$SCALA_HOME/bin
```

`source ~/.bash_profile`をたたいて変更を反映。
`scala -version`をたたいてバージョン情報が出てきたらOK！

# コンパイルと実行
HelloWorld.scalaのコンパイルコマンドは、

```
scalac HelloWorld.scala
```

実行コマンドは、

```
scala -cp . HelloWorld
```

