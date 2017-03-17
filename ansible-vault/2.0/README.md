# Ansible Vault 2.0

```bash
> docker build -t adlawson/ansible-vault:2.0 .
```

```bash
> alias ansible-vault="docker run --rm -it \
    -v `pwd`:/src \
    adlawson/ansible-vault:2.0"

> ansible-vault decrypt --vault-password-file=.ansiblevault path/to/secrets.yml
```
