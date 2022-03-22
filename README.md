### Running tomcat role for installing tomcat in the servers
```
Syntax:
ansible-playbook -i hosts main.yaml -e "env=dev/sit/uat/pt/prod" 
```

### Deploying Artifacts to the infrastructure
```
Syntax:
ansible-playbook -i hosts deploy-cicd.yaml -e "env=dev/sit/uat/pt/prod" -e "version=<versionnumber>" -e "nexus_user=<nexususername>" -e "nexus_password=<nexuspassword>"
```