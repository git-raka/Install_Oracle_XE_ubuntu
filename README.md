# Install_Oracle_XE_Linux

Download oracle repository Database and preinstall in -> [Oracle ](https://www.oracle.com/in/database/technologies/xe-downloads.html)
```
mkdir oracle && cd oracle
wget https://download.oracle.com/otn-pub/otn_software/db-express/oracle-database-xe-21c-1.0-1.ol7.x86_64.rpm
wget https://yum.oracle.com/repo/OracleLinux/OL7/latest/x86_64/getPackage/oracle-database-preinstall-21c-1.0-1.el7.x86_64.rpm
```
<img width="756" alt="image" src="https://user-images.githubusercontent.com/77326619/188308764-2d040524-c39f-4b32-b872-859b97c8d07e.png">

### Yum Local install preinstall first
```
yum -y localinstall oracle-database-preinstall-21c-1.0-1.el7.x86_64.rpm
yum -y localinstall oracle-database-xe-21c-1.0-1.ol7.x86_64.rpm
```
### Disable firewall
```
sudo systemctl stop firewalld
```

### run oracle install
```
/etc/init.d/oracle-xe-21c configure
```

<img width="767" alt="image" src="https://user-images.githubusercontent.com/77326619/188312293-64ca1618-48fe-4b97-8ff0-1bb281aad0a2.png">

