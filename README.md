# 言語処理100本ノック 2020 解法
[言語処理100本ノック](https://nlp100.github.io/ja/)の解法を残します。

## 環境

- Python: 3.6
- Tensorflow: 2.1

Jupyterで開発を行う。

### Run Jupyter Notebook Server

Build docker image

```
$ docker-compose build
```

Run

```
$ docker-compose up
```

Access 0.0.0.0/
Password (default): nlp100

### Change Password

```
$ docker-compose run nlp100 jupyter notebook password
# Enter password:
# Verify password:
# [NotebookPasswordApp] Wrote hashed password to /root/.jupyter/jupyter_notebook_config.json
```
