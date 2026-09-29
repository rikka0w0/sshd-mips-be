Usage:
```sh
curl -L -k -o /tmp/openssh-mipsbe-static-mnt-myvol.tar.gz https://github.com/rikka0w0/sshd-mips-be/releases/download/openssh-mipsbe-static/openssh-mipsbe-static-mnt-myvol.tar.gz
cd /
tar -xzf /tmp/openssh-mipsbe-static-mnt-myvol.tar.gz
/mnt/myvol/usr/bin/ssh-keygen -A
adduser -S -D -H -h /mnt/myvol/var/empty -s /bin/false sshd
chown root:root /mnt/myvol/var/empty
chmod 755 /mnt/myvol/var/empty
```
