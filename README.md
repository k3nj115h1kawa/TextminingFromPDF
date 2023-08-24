# TextminingFromPDF
## 行ったこと
* Pythonでテキストマイニングを行う
* "!pip install --upgrade pip" と "!pip install --upgrade Pillow" の実行 <-- エラー解決のため[7]
* Windows10でSpyder(Python 3.9)を用いて実装
* --> Spyderで可視化を行う際エラーが頻発し, 解決できなかったため, Google Colaboratoryで実装し直した
* --> Google Colaboratory ではデータの読み込みが少し難しい(?) が, 可視化は実行できた
* PDFの内容を読み込み, 形態素解析して可視化できるようにした [1, 2, 3, 5, 6]
* 英数字や記号を取り除き, 日本語の単語のみを可視化対象とするようにした
* 日本語の論文にテキストマイニングを実行してみた --> できた

## 難しかったこと
* ワードクラウドを実行しようとしたとき, 正確に指定しているのに"ValueError: Only supported for TrueType fonts"が表示された [7]
* フォントはTrueTypeフォントであり, フォントのパスも正確に指定して, フォントパスにはスラッシュを用いたがエラーが発生した
* 英単語の削除 <-- 一度, 形態素解析を実行した後のデータフレームの要素から, アルファベットを削除した

## 分かったこと
* 少なくともテキストマイニングの可視化は, Spyderで行うべきではない(おそらく, conda環境自体で行うことが難しい...?) [4] <-- これはGiNZAライブラリであるが, 他の可視化も同様であると思われる
* 形態素解析の実行は, Spyderでも行える

## モチベーション
* 以前, Rで似たようなコード(PDFファイルの内容をテキストマイニングする)を実装したので, Pythonでもやってみた
* Pythonでできるようになると, 他のコードとかとも繋げやすくなりそう(例えば, GUIアプリに組み込むとか)
* Rの方では共起ネットワークを実装できなかったため, Pythonでやってみたかった(<-- Pythonでもできなかった)
* 論文の内容をテキストマイニングしてみたかった

## 参考文献
1. Crystal-Method, "Pythonでテキストマイニングをする方法を詳しく解説します！", "https://crystal-method.com/topics/text-mining_python/" accessed on 2023/08/24
2. BOXCODEADMIN, "NLPLOTが凄い！自然言語を可視化・分析できるPYTHONライブラリ", "https://boxcode.jp/nlplot%E3%81%8C%E5%87%84%E3%81%84%EF%BC%81%E8%87%AA%E7%84%B6%E8%A8%80%E8%AA%9E%E3%82%92%E5%8F%AF%E8%A6%96%E5%8C%96%E3%83%BB%E5%88%86%E6%9E%90%E3%81%A7%E3%81%8D%E3%82%8Bpython%E3%83%A9%E3%82%A4" accessed on 2023/08/24
3. たかぱい@takapy0210, "自然言語を簡単に可視化・分析できるライブラリ「nlplot」を公開しました", "https://www.takapy.work/entry/2020/05/17/192947" accessed on 2023/08/24
4. teratail, "Anaconda環境のpythonでginzaを実行するとエラーメッセージが表示され，解決できない", "https://teratail.com/questions/333577" accessed on 2023/08/24
5. @Drsato_carrer, "pythonで出来るPDF便利技４選【コードあり】", "https://doctorsato.com/python_pdf/" accessed on 2023/08/24
6. narudesu, "前処理、前処理、そして、前処理 （自然言語処理：日本語編）", "https://note.com/narudesu/n/na35de30a583a" accessed on 2023/08/24
7. stackoverflow, "WordCloud Only Supported for TrueType fonts", "https://stackoverflow.com/questions/76129498/wordcloud-only-supported-for-truetype-fonts?rq=2" accessed on 2023/08/24


 
