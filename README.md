FTP using Docker
===============

1. Reference [docker-pure-ftpd](https://github.com/stilliard/docker-pure-ftpd)

### How to create user
```
docker ps # get the container name using this command
docker exec -it <docker-container-name> /bin/bash
pure-pw useradd bob -f /etc/pure-ftpd/passwd/pureftpd.passwd -m -u ftpuser -d /home/ftpusers/bob # follow the instruction to create user + set password
```

### How to use
```
ftp -p localhost 21
```

### FTP command cheatsheet
[the-ultimate-ftp-commands-list](https://www.smartfile.com/blog/the-ultimate-ftp-commands-list/)
