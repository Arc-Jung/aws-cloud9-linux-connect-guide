# Connect at AWS Cloud 9 IDE with all  Linux OS
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FWooSung-Jung%2Faws-cloud9-linux-connect-guide&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
### ***First Commit 2020-06-21 Arc-Jung***

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
   
<img src="https://raw.githubusercontent.com/WooSung-Jung/Connect-AWS-Cloud9-Linux/master/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202020-06-10%20%EC%98%A4%EC%A0%84%2010.16.48.png">

4. Insert Cloud9 IDE environment name with rule For example insert PROJECT_ADMIN_CLOUD9.
5. Rule is PROJECTNAME_PURPOSE_SERVICENAME.
6. Insert USERNAME and HOST IP.

<img src="https://raw.githubusercontent.com/WooSung-Jung/Connect-AWS-Cloud9-Linux/master/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202020-06-10%20%EC%98%A4%EC%A0%84%2010.33.44.png">

7. You are need to add our public key to your instance ~/.ssh/authorized_keys file to select AWS Console Cloud9 button of copy key to SSH key.
-  If you want another directory setting to install your project directory. Insert directory path at Cloud9 console hidden setting.

<img src="https://raw.githubusercontent.com/WooSung-Jung/Connect-AWS-Cloud9-Linux/master/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202020-06-10%20%EC%98%A4%EC%A0%84%2010.33.55.png">

8. Select connect button Cloud9 in AWS console.
9.  Wait 5 minutes while checking the command answering the question.
10. Use Cloud9 on all  Linux OS. For example is Ubuntu, CentOS etc...
11. But Cloud9 user permission will be denied. Insert bash command. ***YOUR DIR*** is your environment setting.

```bash
sudo adduser ubuntu
sudo groupadd cloud9
sudo usermod -a -G cloud9 ubuntu
sudo chown -R ubuntu:cloud9 /<YOUR DIR>
sudo chmod -R 2775 /<YOUR DIR>
```
12. If you have any questions, please write an issue.
