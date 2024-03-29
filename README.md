﻿# Stunnel Demo

このプロジェクトは、Dockerを使用してTLS 1.2およびTLS 1.3をサポートするstunnelサーバーとクライアントのデモ環境を設定するためのものです。これにより、TLS通信の基本的な動作を理解し、テストすることができます。


## 前提条件

- Docker
- Docker Compose

## セットアップ手順

1. リポジトリをクローンします:

   ```bash
   git clone https://github.com/nakasora/stunnel-demo.git
   cd stunnel-demo

## デモ実行
1. Docker Composeを使用してコンテナをビルドし、起動します:
```
docker-compose up --build
```

2. Docker Composeを使用してコンテナをビルドし、起動します:
```
openssl s_client -connect stunnel-demo-stunnel-server-1:443
```

3. サーバコンテナにアタッチして、必要に応じてサーバの設定を確認します:
```
docker exec -it stunnel-demo-stunnel-server-1 bash
```
