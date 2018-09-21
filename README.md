local repo dependency poc (project1 depends on project2)


This demonstrates local development of dependent gradle projects.
- it uses SNAPSHOT version so that the dependency can be updated 
without changing the version parameter.
- it uses maven local repo to store/retrieve the dependency (hence mvn needs to be installed)



to see it in action:

- open Retek.java in project2, change the system out message.
- run gradle install in project2
- run gradle build in project1
- run gradle clean test -i  in project1

your change should be visible.

