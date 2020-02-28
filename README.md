# AWS SES NodeJS Example

Follow the instructions below on an EC2 Ubuntu instance. This tutorial will help you setup the AWS SDK using NodeJS. There are a few endpoints to send email with attachments, create a verified sender, delete a verified sender, and list all of your verified senders. If you have any questions please contact me!

```
sudo su
apt-get update
apt-get upgrade -y
apt-get dist-upgrade -y
apt-get autoremove -y
apt-get install nodejs npm git -y
ln -s /usr/bin/nodejs /usr/bin/node
git clone https://github.com/andrewpuch/aws-ses-node-js-examples.git
cd aws-ses-node-js-examples
npm install
cp config-sample.json config.json
```
```
How To Install Latest Nodejs on Amazon Linux

For Latest Release:-


sudo yum install -y gcc-c++ make
curl -sL https://rpm.nodesource.com/setup_13.x | sudo -E bash -
For Stable Release:-

sudo yum install -y gcc-c++ make
curl -sL https://rpm.nodesource.com/setup_12.x | sudo -E bash -
Step 2 – Install Node.js on Amazon Linux
After adding a yum repository in your system let’s install the Node.js package. NPM will also be installed with node.js. This command will also install many other dependent packages on your system.

sudo yum install -y nodejs
Don’t Miss => Yarn Installation ( A Node Modules Manager)
Step 3 – Check Version
After installation check the installed version of Node.js. You can find more details about current version on node.js official website.

node -v 

v13.9.0
Also, check the version of npm.

npm -v 

6.13.7
```


***NOTE: Here you will want to edit config.json with your AWS keys and in app.js you will want to edit the email address with your own email address. For this tutorial we will just send email to ourselves.***

```
node app.js
```
