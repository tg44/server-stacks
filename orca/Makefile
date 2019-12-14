octoprint-compose=docker-compose -f octoprint.compose.yml -p octoprint
prometheus-compose=docker-compose -f prometheus.compose.yml -p prometheus

default: help

oup: ## Spin up services
	$(octoprint-compose) up -d

ostop: ## Stop services
	$(octoprint-compose) stop

odown: ## Destroy all services and volumes
	$(octoprint-compose) down -v

pup: ## Spin up services
	$(prometheus-compose) up -d

pstop: ## Stop services
	$(prometheus-compose) stop

pdown: ## Destroy all services and volumes
	$(prometheus-compose) down -v
