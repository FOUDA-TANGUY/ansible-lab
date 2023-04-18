
conteners: networks
	docker run -d --network reseau_1 --name contener_1_1 nginx:ssh
	docker run -d --network reseau_2 --name contener_2_1 nginx:ssh

build:
	docker build -t nginx:ssh .ssh/
networks:
	docker network create reseau_1
	docker network create reseau_2
clean:
	docker rm -f contener_1_1 contener_2_1
	docker network rm -f reseau_1 reseau_2

