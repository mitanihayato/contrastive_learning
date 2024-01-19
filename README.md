# 【Qiita】新たな学習方法！「教師あり」Contrastive Learningを解説！
## リンク
[Qiita: Contrastive Learning](https://qiita.com/omiita/items/a9b8b891ae759a75dd42)  

## まとめ
* Contrastive Learningにラベル情報を用いる教師ありCLを提案したよ  
* 教師ありCLで用いる損失関数はSupCon(=Supervised Contrastive)という名前だよ   
* 教師ありCLがクロスエントロピー損失を用いた通常の教師あり学習よりも高い性能を示したよ   
    * ImageNet/CIFAR-10/CIFAR-100の画像分類タスクでより高い分類精度を示したよ   
    * ハイパーパラメーター(e.g. 学習率)への高い安定性も示したよ   
    * ImageNet-Cへのロバスト性もより良いよ

### 用語
温度つきsoftmax(https://qiita.com/nkriskeeic/items/db3b4b5e835e63a7f243)


# 【Qiita】2020年超盛り上がり！自己教師あり学習の最前線まとめ！
## リンク
[Qiita: 自己教師あり学習(2020年)](https://qiita.com/omiita/items/a7429ec42e4eef4b6a4d)

## まとめ
* 自己教師あり学習の最新トレンドはContrastive Learningだよ   
* Contrastive Learningでは、「似ているデータは潜在空間でも似た埋め込みベクトルになり、異なるデータは潜在空間でも異なる埋め込みベクトルになる」ということを学習させるよ   
* Contrastive Learningのアーキテクチャは次の4つに分かれるよ   
    * End-to-End   
    * メモリーバンク  
    * モーメンタムエンコーダー  
    * クラスタリング  
* 自己教師あり学習は、画像分類では教師あり学習にほぼ追いつき、物体検出への転移は教師あり学習よりも良いよ

### 用語
infoNCE Loss: Contrastive Learningで一番有名なLoss

# 参考Github
## SimCLR
pytorch実装  
info nce lossを使用している  
同じclassは無視  
https://github.com/sthalles/SimCLR

## SupContrast: Supervised Contrastive Learning
pytorch実装   
同じclassも考慮してしている  
https://github.com/HobbitLong/SupContrast?tab=readme-ov-file
