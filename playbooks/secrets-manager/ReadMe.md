## General Notes

## Test Locally
### Prereq
1. Ensure that `ansible` is installed locally.
2. Set env vars
```
export AWS_REGION="ap-southeast-2"
export AWS_PROFILE="XXXX"
export DBENV="YYYY"
```
3. Execute Locally
```
no_proxy="*" ansible-playbook secret-verify.yaml
``` 