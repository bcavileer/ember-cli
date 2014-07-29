ember-cli
=========

Docker container that runs ember-cli

docker run -d bcavileer/ember-cli /sbin/my_init --enable-insecure-key

curl -o insecure_key -fSL https://github.com/phusion/baseimage-docker/raw/master/image/insecure_key
chmod 600 insecure_key

ssh -i insecure_key root@<IP address of container>

ember new my-new-app

cd my-new-app
ember server

browse to http://<IP address of container>:4200

