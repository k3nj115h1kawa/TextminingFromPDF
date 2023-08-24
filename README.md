# TextminingFromPDF
## 行ったこと
* Pythonでテキストマイニングを行う
* "!pip install --upgrade pip" と "!pip install --upgrade Pillow" の実行 <-- エラー解決のため
* Windows10でSpyder(Python 3.9)を用いて実装
* --> Spyderで可視化を行う際エラーが頻発し, 解決できなかったため, Google Colaboratoryで実装し直した
* --> Google Colaboratory ではデータの読み込みが少し難しい(?) が, 可視化は実行できた
* PDFの内容を読み込み, 形態素解析して可視化できるようにした
* 英数字や記号を取り除き, 日本語の単語のみを可視化対象とするようにした

## 難しかったこと
* ワードクラウドを実行しようとしたとき, 正確に指定しているのに"ValueError: Only supported for TrueType fonts"が表示された
* フォントはTrueTypeフォントであり, フォントのパスも正確に指定して, フォントパスにはスラッシュを用いたがエラーが発生した
* 英単語の削除 <-- 一度, 形態素解析を実行した後のデータフレームの要素から, アルファベットを削除した

## 分かったこと
* 少なくともテキストマイニングの可視化は, Spyderで行うべきではない(おそらく, conda環境自体で行うことが難しい...?)
* 形態素解析の実行は, Spyderでも行える

## 参考文献
1. 
 
