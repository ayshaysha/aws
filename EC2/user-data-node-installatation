#!/bin/bash
sudo yum update -y
exec > >(tee /var/log/user-data.log|logger -t user-data -s 2>/dev/console) 2>&1
curl --silent --location https://rpm.nodesource.com/setup_14.x | bash -
sudo yum -y install nodejs
