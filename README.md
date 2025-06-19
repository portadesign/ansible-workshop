# Ansible Workshop

Create the `ansible` (the control node) and `webserver` (target node) containers:

```
docker compose up -d
```

Enter the `ansible` container:

```
docker compose exec -it ansible bash
```

Verify Ansible is installed:

```
ansible --version
```

Verify `webserver` is accessible from the `ansible` container via SSH (the password is `root`) by using the `ping` module:

```
ansible webserver -i hosts -m ping --ask-pass
```

Install requirements (roles):

```
ansible-galaxy install -r requirements.yml
```

Run the playbook (use `-vvv` for verbose output):
```
ansible-playbook provision.yml --ask-pass
```
