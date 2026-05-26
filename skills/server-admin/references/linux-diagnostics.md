# Linux Diagnostics

Use these as read-only starting points. Adapt to the distro and service manager.

## System

```bash
hostnamectl
uptime
date -Is
df -h
free -h
top -b -n1 | head -40
```

## Services

```bash
systemctl status <service> --no-pager
journalctl -u <service> -n 100 --no-pager
systemctl list-units --failed --no-pager
```

## Networking

```bash
ss -tulpn
ip addr
ip route
resolvectl status
curl -I http://127.0.0.1:<port>
```

## Disk and Files

```bash
du -xh --max-depth=1 /var 2>/dev/null | sort -h
find /var/log -type f -size +100M -ls 2>/dev/null
ls -lah <path>
```

## Containers

```bash
docker ps
docker logs --tail 100 <container>
docker inspect <container>
```

Do not paste secrets from command output. Summarize sensitive values instead.
