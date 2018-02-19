My version of Dockerized minidlna service.

Configure:
Edit line 10 on "minidlna.docker.service" file:
	change "/media/hdd:" to your local mediafolder path

Build:
	cd minidlna.docker
	docker build -t minidlna.docker .

Install:
	cp minidlna.docker.service /etc/systemd/system/
	systemctl daemon-reload
	systemctl enable minidlna.docker.service
