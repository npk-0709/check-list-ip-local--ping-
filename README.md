# check-list-ip-local--ping-

```bash
for /L %i in (1,1,255) do @ping -n 1 -w 100 192.168.1.%i | findstr "TTL=" | findstr /v "TTL=0"
```
