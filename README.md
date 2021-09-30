# 朝プロ

docker containerでjupyter notebookを開いて作業する。

```sh
docker pull jupyter/scipy-notebook
git clone https://github.com/NaotoKubota/morning-programming-training.git
cd morning-programming-training
docker run -v `pwd`:/home/jovyan/work -p 10000:8888 --name jupyter jupyter/scipy-notebook
```
表示されるtokenをコピーして、ブラウザで `localhost:10000` にアクセスする。

## 資料
- Pythonによる作図
	- [Heatmap](https://github.com/NaotoKubota/morning-programming-training/blob/master/Heatmap.ipynb)
