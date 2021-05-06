build:
	docker-compose build
start:
	docker-compose up -d
stop:
	docker-compose stop
frontend:
	docker-compose exec angular bash
dev-angular:
	docker-compose exec angular bash -c "ng serve --host=0.0.0.0 --disable-host-check"

export prefix=$(shell source .env && echo $$COMPOSE_PROJECT_NAME | tr '[:upper:]' '[:lower:]')
reset:
	docker-compose down || true
	docker volume rm ${prefix}_mongoData || true
	docker-compose up -d --remove-orphans
