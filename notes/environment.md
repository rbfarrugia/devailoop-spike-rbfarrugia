# Environment

Output of two commands, run exactly as written in the ticket.

## 1. `ls -la /run/secrets 2>&1`

```
total 8
drwxr-xr-x 2 nobody nogroup 4096 Oct 13 06:19 .
drwxr-xr-x 1 nobody nogroup 4096 Oct 13 06:19 ..
crw-rw-rw- 1 nobody nogroup 1, 3 Oct 13 06:19 github-app.pem
```

## 2. `test -r /run/secrets/github-app.pem && echo readable || echo not-readable`

```
readable
```
