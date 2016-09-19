##  AWS Elastic Beanstalk

Configuration to create a single T2 instance on elastic beanstalk with forced SSL, running pm2

Features
- HTTPS
- HTTP re-direct to HTTPS (forced SSL)
- Nodejs with PM2 running as --no-daemon

# Deploying
You will need to have created a VPC to use this config as is.

#### Update default.config
Update lines 12 and 15 of `default.config` with VPC and subnet IDs.

#### Update https-instance.config

To use, you need to update the server.crt and server.key in the `https-instance.config` file with your own key and generated csr.
Details on creating self-signed SSL Certificate: http://www.akadia.com/services/ssh_test_certificate.html


