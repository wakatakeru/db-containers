## DB-containers

開発環境向けに、開発用DBを構築します。  
現在、PostgreSQLに対応しています。  

DBクラスタは、プロジェクトルートに保存されるため、永続的です。  
更に、ホストマシンの設定やDBを変更する必要がなくなります。  

### Requirements
- Docker 1.13.0+  
- Docker Compose 1.9.0+  

### Setup
1. localhostの `15432` ポートが使用中でないことを確認  
1. cddir `project-root`  
1. `$ docker-compose up` (デーモナイズが必要な場合は d オプション付与)  

### Usage
#### PostgreSQL
ポートは、`localhost:15432` に開放されています。  
`$ psql -U postgres -h localhost -p 15432` で接続可能です。

