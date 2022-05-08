### Running tomcat role for installing tomcat in the servers
```
Syntax:
ansible-playbook -i hosts main.yaml -e "env=dev/sit/uat/pt/prod" 
```

### Deploying Java Artifacts to the infrastructure
```
Syntax:
ansible-playbook -i hosts deploy-cicd.yaml -e "env=dev/sit/uat/pt/prod" -e "version=<versionnumber>" -e "nexus_user=<nexususername>" -e "nexus_password=<nexuspassword>"
```

### Running dotnet role for installing and configure dotnet in the servers
```
Syntax:
ansible-playbook -i hosts main.yaml -e "env=dev/sit/uat/pt/prod" --ask-pass
Note: Make sure you are giving role name as dotnet
```

### Deploying dotnet Artifacts to the infrastructure
```
Syntax:
ansible-playbook -i hosts deploy-cicd-dotnet.yaml -e "env=dev/sit/uat/pt/prod" -e "artifact_name=<versionnumber>" -e "nexus_user=<nexususername>" -e "nexus_password=<nexuspassword>" --ask-pass
Note: Make sure you are giving role name as deploy-dotnet-cicd
```
