# 朝プロ用資料

docker containerでjupyter notebookを開いて作業する。

```sh
docker pull jupyter/scipy-notebook
git clone git@github.com:NaotoKubota/morning-programming-training.git
cd morning-programming-training
docker run -v `pwd`:/home/jovyan/work -p 10000:8888 --name jupyter jupyter/scipy-notebook
```

- Pythonによる作図
