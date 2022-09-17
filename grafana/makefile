SHELL := /bin/bash
.PHONY:	up down build rebuild

up:
	docker-compose up

down:
	docker-compose down

build:
	docker-compsoe build

rebuild:
	docker-compose down
	docker image rm grafana/grafana
	docker-compose build
	docker-compose up
