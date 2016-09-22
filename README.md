# ec2-simple-test
Test application for (AWS) Elastic Beanstalk, and a few other AWS services.

## Useful Commands

### Simple S3 deployment
```
mvn clean package -Ps3 - simple s3 deployment
```

### Create Beanstalk environment
```
eb create --cfg demo-tomcat7 -p tomcat-7-java-7 -c ec2-simple-dev ec2-simple-dev 
```

## Maven Profiles
* redis - enables redis
* s3 - adds ebextensions config to auto-deploy s3
* memcache - adds ebextensions config, and libs, to allow memcache to be the session manager

