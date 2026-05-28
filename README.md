# MLLearn

『Attention Is All You Need』を読めるようになるために、機械学習の基本を順番に学ぶための教材です。

最初から Transformer の数式へ進むのではなく、入力と出力、モデル、パラメータ、損失関数、勾配降下法、分類、回帰、確率、表現学習、ニューラルネットワークを積み上げて、最後に Transformer へ接続します。

## まず読むもの

- [リンク付き目次](Table%20of%20Contents.md): 全章と節へ移動するための目次
- [用語集](Glossary.md): 章を読む途中で確認したい基本語の一覧
- [memo.txt](memo.txt): この教材を作るきっかけと方針メモ

## 読み方

1. [第1章 機械学習とは何か](Chapter%201%20What%20Is%20Machine%20Learning.md) から順番に読む
2. 各章の Mermaid 図で概念の流れを確認する
3. PyTorch サンプルコードを手元で少し変えて動かす
4. 各章末の「Transformer への接続」と「ミニ演習」で理解を確認する
5. [第14章 Transformer を読むために必要な機械学習知識](Chapter%2014%20Machine%20Learning%20Knowledge%20Required%20to%20Read%20Transformer.md) まで読んで、Attention の式に戻る

## 構成

- 第1章から第7章: 機械学習の基本構造、損失、最適化、汎化
- 第8章から第11章: 分類、回帰、特徴量、確率
- 第12章: ニューラルネットワークへの橋渡し
- 第13章: 機械学習システム全体の流れ
- 第14章: Transformer と `Attention Is All You Need` への接続

## 実行環境

章内のサンプルコードは、Python と PyTorch で動かすことを想定しています。

```bash
python3 -c "import torch; print(torch.__version__)"
```

コードは小さな確認用なので、GPU は不要です。CPU だけで動くようにしています。

## この教材で重視していること

- 数式より先に、何を入力し、何を出力し、何を正解としているかを見る
- 予測、損失、勾配、パラメータ更新の流れを何度も確認する
- softmax、交差エントロピー、embedding、Self-Attention を Transformer への橋として理解する
- 章ごとに図、コード、ミニ演習で同じ概念を別の角度から見る

## 次に作るとよさそうなもの

- `examples/` ディレクトリに、章内コードを実行用 Python ファイルとして分離する
- Transformer を小さく実装する章または別冊を作る
- `Attention Is All You Need` の Figure 1 と Section 3.2 を読み解くノートを作る
