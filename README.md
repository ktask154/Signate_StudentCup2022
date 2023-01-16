# Signate_StudentCup2022

## 課題
英語圏の求人情報に含まれるテキストデータをもとに、その職務内容が①データサイエンティスト、②機械学習エンジニア、③ソフトウェアエンジニア、④コンサルタント のどの職種に該当するかを判別するアルゴリズムを構築する。

[link](https://signate.jp/competitions/724#abstract)

### 評価関数
F1score （マクロ平均）


## Models
- Deberta-v3-large
- Deberta-v3-base
- Deberta-large
- RoberTa-large

## work
- StratifiedKFold(jobflag) Fold=5
- CrossEntropyLoss
- AdamW
- Pooler Output
  - Mean Pooling
  - Attention Pooling
- epoch : 10

