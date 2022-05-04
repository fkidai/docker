
#セットアップ
#wslから以下を実行
cd docker
docker-compose build
docker-compose up -d

#以下のサイトにアクセスして利用
http://localhost:3333/

#全て削除
cd docker
docker-compose down --rmi all --volumes --remove-orphans
