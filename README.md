# sap_test
#CodeDeploy test
#user data for dependencies installation for AWS
#!bin/bash
sudo yum update
sudo yum install -y ruby
sudo yum install wget
wget https://aws-codedeploy-ap-southeast-2.s3.ap-southeast-2.amazonaws.com/latest/install
chmod +x ./install
sudo ./install auto
sudo service codedeploy-agent start 
sudo yum install -y python-pip
sudo pip install awscli
