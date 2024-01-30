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

- ***Update the `application.properties` file with your database details:***
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

4. **Go to: http://localhost:8080**


## Project Strucutre 

```bash
├── .devcontainer
│   ├── Dockerfile
│   └── devcontainer.json
├── .gitignore
├── README.md
├── data
├── mvnw
├── mvnw.cmd
├── pom.xml
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com
│   │   │       └── studio
│   │   │           └── climatechange
│   │   │               ├── ClimateChangeApplication.java                - Main Application entrypoint for **Spring Boot**
│   │   │               ├── Helper.java
│   │   │               ├── JDBCConnection.java
│   │   │               ├── controller
│   │   │               │   ├── AboutController.java
│   │   │               │   ├── ChangesInPeriodsController.java
│   │   │               │   ├── ChangesInRegionsController.java
│   │   │               │   ├── Level1SubtaskAController.java
│   │   │               │   ├── Level2SubtaskBController.java
│   │   │               │   ├── Level2subtaskAcontroller.java
│   │   │               │   ├── SimilarPeriodsController.java
│   │   │               │   └── SimilarRegionsController.java
│   │   │               ├── dto
│   │   │               ├── models
│   │   │               │   ├── City.java
│   │   │               │   ├── Country.java
│   │   │               │   ├── Global.java
│   │   │               │   ├── Persona.java
│   │   │               │   ├── Population.java
│   │   │               │   ├── State.java
│   │   │               │   ├── Student.java
│   │   │               │   └── Temperature.java
│   │   │               ├── repository
│   │   │               ├── services
│   │   │               └── viewModel
│   │   │                   ├── level2SubtaskA
│   │   │                   ├── level2SubtaskB
│   │   │                   ├── level3SubtaskA
│   │   │                   ├── level3SubtaskB
│   │   │                   └── level3SubtaskBPart2
│   │   └── resources
│   │       ├── application.properties
│   │       ├── data
│   │       ├── images
│   │       ├── static
│   │       │   ├── functions
│   │       │   ├── images
│   │       │   └── styles
│   │       └── templates
│   │           ├── LandingPage.html
│   │           ├── Lv2-Subtask-B.html
│   │           ├── about.html
│   │           ├── changesInPeriods.html
│   │           ├── changesInRegions.html
│   │           ├── level2subtaskA.html
│   │           ├── similarPeriods.html
│   │           └── similarRegions.html
│   └── test
│       └── java
│           └── com
│               └── studio
│                   └── climatechange
│                       └── ClimateChangeApplicationTests.java
└── target
    ├── classes
    ├── generated-sources
    ├── generated-test-sources
    ├── maven-status
    └── test-classes
```


## Authors
**Nguyen Doan Trung Truc (s3974820)**
**Ho Tuan (s4019549)**
**On Tuan Huy (s4028018)**
**Lam Manh Tuan (s4037166)**
**Le Duc Huy (s4040502)**

## Copyright RMIT University (c) 2024 



