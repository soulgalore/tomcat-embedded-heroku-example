# Example project for deploying Tomcat on Heroku
This is an example setup to run Tomcat on Heroku. Now it uses the webapp-runner from jsimone.

# Running it local
```mvn clean install```

```java -jar target/dependency/webapp-runner.jar target/*.war```

# Running within Eclipse
https://github.com/jsimone/webapp-runner

# Deploying 

1. Checkout this project
2. Add it to Heroku ```heroku create --stack cedar```
3. Rename your project to whatever name you want, in this exanmple we will use tomcat-tst ```heroku rename tomcat-tst```
4. Add the Heroku as a remote ```git remote add heroku git@heroku.com:tomcat-tst.git```
5. Push it: ```git push heroku master```
6. Access your application: http://tomcat-tst.herokuapp.com/