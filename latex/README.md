# 卒論テンプレート（LaTeX）

$LaTeX$ を用いて卒論を書く場合に用いてください．

## 使い方

卒論執筆のために編集しなければいけないファイルは `thesis.tex` と `thesis.bib` の2つです．
`thesis.tex`に，卒論の本文を，`thesis,bib`には参考文献を $BibTeX$形式で記入します．


* コンパイル
  * `llmk` コマンドを実行することで，`thesis.pdf` が作成されます．
* 不要なファイルを削除する．
  * `llmk -c` もしくは `llmk --clean`
    * 不要な中間ファイルを削除する．最終成果物は残したまま．
  * `llmk -C` もしくは `llmk --clobber`
    * `llmk`コマンドで作成されたすべてのファイルを削除する．

初回編集時に，`thesis.tex` の次の項目を修正してください．

* **18行目**　卒論のタイトルを書いてください．
* **22, 23行目** 学位の種別を適切なものに変更してください（学士 or 修士）．
* **27行目**　あなたの名前に置き換えてください．
* **34行目**　卒業年度を適切に置き換えてください．
* **37〜41行目**　所属学部，研究科を適切なものにしてください．
* **44行目**　学生証番号を記入してください．
* **47行目**　指導教員の名前に置き換えてください．

## $LaTeX$

### インストール

詳細は [$TeX$ Wiki](https://texwiki.texjp.org/?TeX%20Live%2FMac#install) をご覧ください．
数ギガバイト単位のファイルをダウンロードするため，テザリング状態では実行しないようにしてください．

#### GUIありの場合

```sh
brew install --cask mactex
sudo tlmgr update --self --all
sudo tlmgr paper a4
```

#### GUIなしの場合

```sh
brew install --cask basictex
sudo tlmgr update --self --all
sudo tlmgr paper a4
sudo tlmgr install collection-langjapanese
```

## リンク

* [$LaTeX$入門](https://texwiki.texjp.org/?LaTeX入門)
* [$BibTeX$入門](http://mikilab.doshisha.ac.jp/dia/seminar/latex/doc/bib.html)

