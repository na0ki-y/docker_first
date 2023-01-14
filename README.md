# docker_first

# OverView　
dockerでpythonの環境を構築するサンプルです。
docker内にpython,pipenv環境を作り、numpyの動作確認を行います。

# Installation :balloon:
## 環境設定
```bash
brew install --cask docker
docker pull python:3
```
## clone/dockerイメージの作成
```bash
git clone git@github.com:na0ki-y/docker_first.git
cd docker-python/
sudo docker compose up -d --build
```
## 接続
```bash
docker compose exec サービス名 bash
docker exec -it コンテナ名 /bin/bash
```
## sampleの実行
```bash
cd opt 
pipenv install
pipenv shell
python sample.py
```