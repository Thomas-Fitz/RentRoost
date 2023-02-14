## Database

Inside the database directory, you'll find an executable Bash script (`.sh` file) and several SQL scripts (`.sql` files). These can be used to build and rebuild a PostgreSQL database for the capstone project.

From a terminal session, execute the following commands:

```
cd <project-root>/database/
./create.sh
```

This Bash script drops the existing database, if necessary, creates a new database named `final_capstone`, and runs the various SQL scripts in the correct order. You don't need to modify the Bash script unless you want to change the database name.

## Spring Boot
Note: Spring Boot has been configured to run on port `9000` for this project. You might be used to port `8080` from earlier in the cohort, but it's changed so as not to conflict with the Vue server that you'll be running concurrently.

### Datasource

A Datasource has been configured for you in `/src/resources/application.properties`. It connects to the database using the `capstone_appuser` database user. You can change the name of this database if you want, but remember to change it here and in the `create.sh` script in the database folder:

```
# datasource connection properties
spring.datasource.url=jdbc:postgresql://localhost:5432/final_capstone
spring.datasource.name=final_capstone
spring.datasource.username=final_capstone_appuser
spring.datasource.password=finalcapstone
```
