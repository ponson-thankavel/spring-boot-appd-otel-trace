1. First clone the project to your local

```console
git clone <<repo-url>> .
```

2. Open the project in your IDE (ex: IntelliJ Idea)
3. Deploy Grafana & Tempo to your local (you can use [tempo-grafana-docker-compose](https://github.com/ponson-thankavel/tempo-grafana-docker-compose))
4. Download appd appagent 22.3+ to your local directory
5. Update pom.xml
   1. Set parameters in ```jvmArguments``` section as mentioned
6. Build and run
7. Access application home at ```http://localhost:8080/``` a few times to generate some traffic
8. Verify application in your appdynamics saas controller
9. Pick-up TraceId from application logs in IDE and verify traces in Tempo source by opening Grafana
