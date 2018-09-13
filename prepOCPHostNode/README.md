# Playbook to prep Openshift Host nodes


## Execution
```
ansible-playbook -v -i hosts -e "target=NODE_GROUPNAME" -e "user=ec2-user" -e "rh_password=INSERT_PWD" -e "rh_username=INSERT_USERNAME" playbook.yml -t test
```

## Testing only
```
ansible-playbook -v -i hosts -e "target=NODE_GROUPNAME" -e "user=ec2-user" -e "rh_password=INSERT_PWD" -e "rh_username=INSERT_USERNAME" playbook.yml
```
