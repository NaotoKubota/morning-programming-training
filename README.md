# 朝プロ

火・木 9:30 ~ 10:00

## 準備
Docker で Jupyter notebookを開く。

```Bash
docker pull jupyter/scipy-notebook
git clone https://github.com/NaotoKubota/morning-programming-training.git
cd morning-programming-training
docker run --rm -v `pwd`:/home/jovyan/work -p 10000:8888 --name jupyter jupyter/scipy-notebook
```
表示されるtokenをコピーして、ブラウザで `localhost:10000` にアクセスする。

## 資料
- Pythonによる作図
	- [Heatmap](https://github.com/NaotoKubota/morning-programming-training/blob/master/Heatmap.ipynb)
	- [Barplot](https://github.com/NaotoKubota/morning-programming-training/blob/master/Barplot.ipynb)

## 参考URL
- [Dockerを使って5分でJupyter環境を構築する](https://qiita.com/fuku_tech/items/6752b00770552bf4f46b)
