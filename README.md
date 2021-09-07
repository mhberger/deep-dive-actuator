Simple grails project to demonstarate Spring Boot Actuator
==========================================================


Build and rung the app using

```
./gradlew clean assemble
cd build/libs/
./t4012_actuator-0.1.jar
```

Then call on actuator/info

```
curl http://localhost:8080/actuator/info

  {"app":{"name":"t4012_actuator","version":"0.1","grailsVersion":"4.0.12"},"build":{"version":"0.1","artifact":"t4012_actuator","name":"t4012_actuator","group":"t4012_actuator","time":1631027993.047000000}}
```
Note that build.time is returned as a float e.g. `1631027993.047000000`.

The question is how to configure Grails/Spring Boot so that the build.time is formatted as `'yyyy-MM-DD hh:mm:ss'`?
