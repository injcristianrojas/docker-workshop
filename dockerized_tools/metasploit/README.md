# Docker Metasploit HOWTO

(based to the defunct tutorial by [A White Hatter](https://web.archive.org/web/20180822221930/http://awhitehatter.me/howto-running-the-metasploit-framework-with-the-native-docker-compose-file/))

Create a local .msf4 directory:

```shell
mkdir ~/.msf4
```

Now launch the stack as a daemon application:

```shell
docker-compose up -d
```

Now run the MSFconsole:

```shell
docker-compose run -p 8880:8880 ms
```

You can also run other MSF utilities, like msfvenom:

```shell
docker-compose run ms ./msfvenom [options]
```