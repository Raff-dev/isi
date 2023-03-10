# [ISI](../README.md) Camunda Spring Boot Application
Spring Boot Application using [Camunda](http://docs.camunda.org).

This project has been generated by the Maven archetype
[camunda-archetype-spring-boot-7.18.0](https://docs.camunda.org/manual/latest/user-guide/process-applications/maven-archetypes/).

---

## API usage

POST  http://localhost:8080/engine-rest/process-definition/key/Process_0j3mwpk/start

```json
{
    "variables":{
        "hour": {"value":"12"},
        "desired_language": {"value":"pl"}
    },
     "withVariablesInReturn": true
}
```

#

## Running the application
1. Build the application using:

```bash
# build the application
mvn clean package

# run the *.jar file from the `target` directory
java -jar target/partyOrganizer.jar
```
or

```bash
# Build and deploy the process application
mvn clean package spring-boot:run
```
or

Run the project as a Java application in your IDE using CamundaApplication as the main class.

---

### Run and Inspect with Tasklist and Cockpit
Once you deployed the application you can run it using
[Camunda Tasklist](http://docs.camunda.org/latest/guides/user-guide/#tasklist)
and inspect it using
[Camunda Cockpit](http://docs.camunda.org/latest/guides/user-guide/#cockpit).

# Show me the important parts!
[BPMN Process](src/main/resources/process.bpmn)

## Environment Restrictions
Built and tested against Camunda Platform version 7.18.0.
