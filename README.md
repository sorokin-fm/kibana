Professional alternative to log files is a log service of course. And if you're using docker, it's not about alternative, it's only reasonable way.

So, you don't want to pay for saas and want to use your own server for this purpose? Follow these steps:

- сlone reepository
- сopy .env file from .env-example and set your own project name
- Go to http://www.htaccesstools.com/htpasswd-generator/ and create your credentials to login, then write it down to .docker/nginx/htpasswd . By default there admin:admin credential
- run docker-compose up -d

That's all!

Based on https://github.com/deviantony/docker-elk

