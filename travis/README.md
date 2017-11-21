# Ansible Vault 2.0

```bash
> docker build -t adlawson/travis .
```

```bash
> alias ansible-vault="docker run --rm -it \
    -v `pwd`:/src \
    adlawson/travis"

> travis encrypt SOMEVAR="secretvalue"
```
