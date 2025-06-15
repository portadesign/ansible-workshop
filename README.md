# Ansible Workshop

Create the `ansible` (the control node) and `webserver` (target node) containers:

```
docker compose up -d
```

Enter the `ansible` container:

```
docker compose exec -it ansible bash
```

Verify `webserver` is accessible from the `ansible` container via SSH (the password is `root`):

```
ssh root@webserver
```