# Citation-Network-Analysis
## 資料集
本研究運用訊息傳播（retweet prediction）預測模型於學術資料集，使用的學術文獻資料集由Aminer平台整理，包含DBLP(Digital Bibliography & Library Project)、MAG (Microsoft Academic Graph)、ACM(Association for Computing Machinery)等數個組織計劃的開放資料。

> 網站：https://www.aminer.cn/citation

每一篇文獻包含以下資料，各個版本資料集的metadata詳細程度不同。
1. paperTitle：標題
2. Authors：作者
3. publication venue：出版平台
4. index id of this paper：在這個資料集中的id
5. the id of references of this paper：引用的其他文獻的id
6. Abstract：摘要
7. n_citation：被引用次數

## 問題定義
若研究者引用某一篇文獻，視為研究者轉發（retweet）該文獻。給定一組「文獻」-「作者」的配對，預測是否會引用該文獻（二元分類問題）。