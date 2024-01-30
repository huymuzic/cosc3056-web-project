# Climate Change Studio Project

Welcome to the Climate Change Studio project! This Spring Boot application provides a platform for developing a climate-related data handling website application.

## Before you begin, ensure you have the following installed:

- Java 17 or later
- [MySQL](https://dev.mysql.com/downloads/) (for database operations)
- [Maven](https://maven.apache.org/download.cgi) (for building the project)


## Getting Started

Follow these steps to get the project up and running on your local machine.

1. **Clone the repository:**

```bash
git clone git@github.com:RMIT-Vietnam-Teaching/cosc3056-studio-project-team-sg01-g02-cosc3056.git
cd cosc3056-studio-project-team-sg01-g02-cosc3056
```

2. **Configure Database:**

- ***Run your MYSQL in local with port 3306***

- ***Create a MYSQL database named `climatechange`***

- ***Update the application.properties file with your database details:***
```
spring.datasource.url=jdbc:mysql://localhost:3306/climatechange
spring.datasource.username=your_database_username
spring.datasource.password=your_database_password
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.hibernate.ddl-auto=update

spring.jpa.show-sql=true
```

3. **Build and Run the Application:**
```bash
mvn spring-boot:run
```


## LICENCE 

This section provides users with Maven commands they can use to clean and build the project, run tests, package the application, and run the packaged JAR file. Adjust the commands based on your project's specific requirements.




