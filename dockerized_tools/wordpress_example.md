Wordpress example

Go to vulnerable Wordpress and launch:

```shell
docker run --name vulnerablewordpress -d -p 80:80 -p 3306:3306 wpscan/vulnerablewordpress
```

Find out machine IP:

```shell
docker inspect -f "{{ .NetworkSettings.IPAddress }}" vulnerablewordpress
```

Launch dockerized wpscan:

docker run -it --rm wpscanteam/wpscan --url http://<MACHINE_IP> --wp-content-dir /  --enumerate u
