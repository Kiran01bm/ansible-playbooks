# Playbook to create, configure and mount a LVM based filesystem

## Execution
```
ansible-playbook -kv -i hosts -e "user=root" -e "target=SERVER_NAME" -e "pv_name=/dev/sdb1" -e "mnt_point=/app_home"  -e "vg_name=app-vg" -e "lv_name=app-pool" playbook.yml
```

## Testing only
```
 ansible-playbook -kv -i hosts -e "user=root" -e "target=SERVER_NAME" -e "pv_name=/dev/sdb1" -e "mnt_point=/app_home"  -e "vg_name=app-vg" -e "lv_name=app-pool" playbook.yml -t test
```
