##### docker-compose up -d
##### docker exec -it rabbitmq2 rabbitmqctl stop_app
##### docker exec -it rabbitmq2 rabbitmqctl reset
##### docker exec -it rabbitmq2 rabbitmqctl join_cluster rabbit@rabbitmq-1
##### docker exec -it rabbitmq2 rabbitmqctl start_app

##### docker exec -it rabbitmq3 rabbitmqctl stop_app
##### docker exec -it rabbitmq3 rabbitmqctl reset
##### docker exec -it rabbitmq3 rabbitmqctl join_cluster rabbit@rabbitmq-1
##### docker exec -it rabbitmq3 rabbitmqctl start_app


#### localhost:15672 접속 후 확인
ID : admin
PW : 1234
