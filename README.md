# zabbix-installation-with-docker

This Docker Compose file sets up a complete Zabbix monitoring stack, including a MySQL database, Zabbix server, Zabbix frontend, Grafana, and a Zabbix agent.

Services :

1-MySQL: A MySQL 5.7 database for storing Zabbix data.
2-Zabbix Server: The Zabbix server component, connected to the MySQL database.
3-Zabbix Frontend: The Zabbix web interface, also connected to the MySQL database.
4-Grafana: A data visualization tool, integrated with the Zabbix server.
5-Zabbix Agent: A Zabbix agent container for monitoring the host system.

Usage : 

1-Clone the repository or copy the docker-compose.yml file to your desired location.
2-Run docker-compose up -d to start the containers.
3-Access the Zabbix frontend at http://localhost and the Grafana dashboard at http://localhost:3000.

Configuration :

1-The MySQL database credentials are set in the environment variables of the mysql service.
2-The Zabbix server and frontend are configured to use the MySQL database with the same credentials.
3-The Grafana container is set to install the Zabbix plugin.
4-The Zabbix agent is configured to connect to the Zabbix server at the IP address 127.0.0.1 (IP Public of your server).

How to running :

for running this compose file you need to run this command in your shell :

docker compose up -d 

###Repository Structure
zabbix-docker
├── README.md
├── docker-compose.yml
└── .gitignore




