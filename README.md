# Connect at AWS Cloud 9 IDE with all  Linux OS

### ***First Commit 2020-06-21 WooSung-Jung***

## Connect and run in remote server (SSH) with all  Linux OS
1. Connect SSH to instance and Insert bash command.
```bash
sudo apt-get install --fix-broken 
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install nodejs
sudo apt-get install nodejs-legacy
```
2. Login to AWS Console.
3. Select Cloud9.
4. Insert Cloud9 IDE enviroment name with rule For example insert PROJECT_ADMIN_CLOUD9.
5. Rule is PROJECTNAME_PURPOSE_SERVICENAME.
6. Insert USERNAME and HOST ip adress.
7. You are need to add our public key to your instance ~/.ssh/authorized_keys file at AWS Console Cloud9 SSH key.
8. Select connect button Cloud9 in AWS console.
9. Wait 5 minutes while checking the command answering the question.
10. Use Cloud9 on all  Linux OS.