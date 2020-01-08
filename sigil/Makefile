file-compose=docker-compose -f file-server.compose.yml -p file-server
hassio-compose=docker-compose -f hassio.compose.yml -p hassio-server
utility-compose=docker-compose -f utility.compose.yml -p utility-server

default: help

fup: ## Spin up services
	$(file-compose) up -d

fstop: ## Stop services
	$(file-compose) stop

fdown: ## Destroy all services and volumes
	$(file-compose) down -v

hup: ## Spin up services
	$(hassio-compose) up -d

hstop: ## Stop services
	$(hassio-compose) stop

hdown: ## Destroy all services and volumes
	$(hassio-compose) down -v

uup:
	$(utility-compose) up -d

ustop:
	$(utility-compose) stop

udown:
	$(utility-compose) down -v
