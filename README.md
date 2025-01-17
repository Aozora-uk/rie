<h1><p align="center"><img src="./rieicon.png" alt="りえ" height="200"></p></h1>
<p align="center">An Rie for AZPick(Cherrypick) & Misskey. <a href="./torisetu.md">About Rie</a></p>

## これ何ですの
Aozora.ukがsyuilo/aiをフォークして制作中のAZPick(Cherrypick)&Misskey用の日本語Botです。

## インストール
> Node.js と npm と MeCab (オプション) がインストールされている必要があります。

まず適当なディレクトリに `git clone` します。
次にそのディレクトリに `config.json` を作成します。中身は次のようにします:
``` json
{
	"host": "https:// + あなたのインスタンスのURL (末尾の / は除く)",
	"i": "藍として動かしたいアカウントのアクセストークン",
	"master": "管理者のユーザー名(オプション)",
	"notingEnabled": "ランダムにノートを投稿する機能を無効にする場合は false を入れる",
	"keywordEnabled": "キーワードを覚える機能 (MeCab が必要) を有効にする場合は true を入れる (無効にする場合は false)",
	"chartEnabled": "チャート機能を無効化する場合は false を入れてください",
	"reversiEnabled": "藍とリバーシで対局できる機能を有効にする場合は true を入れる (無効にする場合は false)",
	"serverMonitoring": "サーバー監視の機能を有効にする場合は true を入れる (無効にする場合は false)",
	"mecab": "MeCab のインストールパス (ソースからインストールした場合、大体は /usr/local/bin/mecab)",
	"mecabDic": "MeCab の辞書ファイルパス (オプション)",
	"memoryDir": "memory.jsonの保存先（オプション、デフォルトは'.'（レポジトリのルートです））"
}
```
MeCabの辞書はもちろんNeologd使ってもいいのですがmecab-ipadic-utf8のほうがお手軽でいいです

`npm install` して `npm run build` して `npm start` すれば起動できます

Nodejsのバージョンが古いと動かないので注意です。アプデしましょう

## フォント
一部の機能にはフォントが必要です。藍にはフォントは同梱されていないので、ご自身でフォントをインストールディレクトリに`font.ttf`という名前で設置してください。

font.ttfには<a href="https://moji.or.jp/ipafont/ipafontdownload/">IPAexゴシック</a>がおすすめです。

## 記憶
りえは記憶の保持にインメモリデータベースを使用しており、りえのインストールディレクトリに `memory.json` という名前で永続化されます。

## ライセンス
MIT

## Awards
<img src="./WorksOnMyMachine.png" alt="Works on my machine" height="120">
