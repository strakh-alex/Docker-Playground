My version of Dockerized transmission daemon.

Configure:
Edit settings.json your preferable setting

Build:
	cd transmission.docker
	docker build -t transmission.docker .

Install:
	cp transmission.docker.service /etc/systemd/system/
	systemctl daemon-reload
	systemctl enable transmission.docker.service
