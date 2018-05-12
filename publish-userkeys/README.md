# Simple playbook to publish users public keys to ssh enabled servers


## Execution
```
ansible-playbook -kv -i inventory -e "target=SERVERS_LIST" -e "user=USERNAME" playbook.yml
```

## Testing only
```
ansible-playbook -kv -i inventory -e "target=SERVERS_LIST" -e "user=USERNAME" playbook.yml -t test
```
