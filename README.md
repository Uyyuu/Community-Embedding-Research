# ML_templete

研究で使う python のデータ分析環境

## ディレクトリ構成

```
.
├── README.md
├── data
│   ├── processed       #前処理済みのデータ
│   └── raw             #生データ
├── docker
│   └── Dockerfile
├── docker-compose.yaml
├── models              #学習済みのモデルやモデルのアーキテクチャ
├── notebooks           #Jupyter notebook
│   └── sample.ipynb
├── outputs             #アウトプット
│   ├── figures         #図や表
│   └── images          #画像
├── poetry.lock
├── pyproject.toml
└── src
    ├── __init__.py
    ├── data            #データ生成やダウンロード
    ├── features        #特徴量エンジニアリング
    ├── models          #学習・推論
    └── visualization   #可視化
```

## セットアップで詰まったところ

- .env ファイルの `COMPOSE_PROJECT_NAME` を設定する．(**大文字使わない！**)
- `docker-compose.yaml`内のML_templeteって部分を変更する
- `.devcontainer/devcontainer.json`の`workspaceFolder`を`docker-compose.yaml`のvolumesと統一する．

## 参考サイト

- [ディレクトリ構成](https://zenn.dev/pluck/articles/63413cdd51f790)
