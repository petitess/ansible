ansible-playbook --inventory hosts main-playbook.yml

# Run playbook

```bash
ansible-playbook --inventory hosts main-playbook.yml
```

```bash
ansible-playbook --inventory hosts main-playbook.yml -v
```

## Run playbook with run time variables

```bash
ansible-playbook --inventory hosts main-playbook.yml --extra-vars '{"version":"1.0","other_variable":"foo-world"}' 
```

## Run playbook with vars from YAML file

```bash
ansible-playbook --inventory hosts main-playbook.yml --extra-vars "@my-vars.yml"
```

```bash
ansible-playbook playbook.yml 
--extra-vars '{"version":"1.0"}' 
```