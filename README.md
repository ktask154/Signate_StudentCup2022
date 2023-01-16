# Signate StudentCup 2022

## 課題
英語圏の求人情報に含まれるテキストデータをもとに、その職務内容が①データサイエンティスト、②機械学習エンジニア、③ソフトウェアエンジニア、④コンサルタント のどの職種に該当するかを判別するアルゴリズムを構築する。
[link](https://signate.jp/competitions/724#abstract)

### 評価関数
F1score （マクロ平均）

</br>

## Models
- Deberta-v3-large
- Deberta-v3-base
- Deberta-large
- RoberTa-large

</br>

## Work
- Resolve encoding error
- htmlタグの除去
- 重複データの除去
- StratifiedKFold(jobflag) Fold=5
- CrossEntropyLoss
- AdamW
- Pooler Output
  - Mean Pooling
  - Attention Pooling
- epoch : 10
- stacking(LGBM,CTB,logistic)
- 最頻値でアンサンブル

</br>

## Result
### 最終提出
5 / 221  位（繰り上げで3位入賞）

public LB : 0.762

private LB : 0.755
</br>
</br>
### ベストシングルモデル(exp20)
 cv : 0.730 
 
 public LB : 0.750
 
 private LB : 0.759


