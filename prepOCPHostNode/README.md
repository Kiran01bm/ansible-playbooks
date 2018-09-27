# Playbook to prep Openshift Host nodes


## Dry-run, In skip-tags use rpmized for container-based installation and containerized for rpm-based installation
```
ansible-playbook -v -i hosts --skip-tags "rpmized" -e "target=NODE_GROUPNAME" -e "user=ec2-user" -e "rh_password=INSERT_PWD" -e "rh_username=INSERT_USERNAME" -e "docker_version=INSERT_DOCKER_VERSION" -e "block_device_name=DEVICE_NAME" playbook.yml -t test
```

## Execution, In skip-tags use rpmized for container-based installation and containerized for rpm-based installation
```
ansible-playbook -v -i hosts --skip-tags "rpmized" -e "target=NODE_GROUPNAME" -e "user=ec2-user" -e "rh_password=INSERT_PWD" -e "rh_username=INSERT_USERNAME" -e "docker_version=INSERT_DOCKER_VERSION" -e "block_device_name=DEVICE_NAME" playbook.yml
```
