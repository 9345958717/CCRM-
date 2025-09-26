# 📘 Campus Course & Records Manager (CCRM)

## 🔹 Project Overview

Campus Course & Records Manager (CCRM) is a Java SE console-based application designed to simplify the management of academic records in a campus environment. The system enables administrators to efficiently handle student data, course offerings, enrollments, grades, and transcripts in a structured way.

- Unlike a simple CRUD app, CCRM also integrates:
- CSV Import/Export for easy data portability
- Backup & Archiving utilities using Java NIO.2
- Validation & Recursive utilities for clean data handling
- GPA computation & Transcript generation with automatic grade assignment

##### The project demonstrates core Object-Oriented Programming concepts (Encapsulation, Inheritance, Abstraction, Polymorphism) along with modern Java features such as Streams API, Date/Time API, exception handling, assertions, and design patterns (Singleton, Builder).

---

## 📂 Project Structure
```text
CCRM/
├─ data/
│  ├─ students.csv
│  └─ courses.csv
└─ src/
   └─ edu/
      └─ ccrm/
         ├─ cli/
         │  └─ CampusCourseRecordsManager.java
         ├─ domain/
         │  ├─ Person.java
         │  ├─ Student.java
         │  ├─ Instructor.java
         │  ├─ Course.java
         │  ├─ Enrollment.java
         │  ├─ Transcript.java
         │  ├─ Semester.java
         │  ├─ Grade.java
         │  └─ CourseCode.java
         ├─ service/
         │  ├─ StudentService.java
         │  ├─ CourseService.java
         │  ├─ EnrollmentService.java
         │  └─ TranscriptService.java
         ├─ io/
         │  ├─ ImportExportService.java
         │  └─ BackupService.java
         ├─ util/
         │  ├─ DataLoader.java
         │  ├─ Validators.java
         │  └─ RecursionUtils.java
         └─ config/
            └─ AppConfig.java
```


---

## ▶️ How to Run

### ✅ Prerequisites

- JDK 17 or later
- Any IDE (VS Code/Eclipse/IntelliJ) or CLI terminal

### 🖥 Compile

From the project root, run:

```sh
javac -d out src/edu/ccrm/cli/*.java src/edu/ccrm/service/*.java src/edu/ccrm/io/*.java src/edu/ccrm/domain/*.java src/edu/ccrm/util/*.java src/edu/ccrm/config/*.java
```
---

### Sample CSV Data
#### students.csv
```sh
1,REG1001,Ananya Sharma,ananya@example.com,true
2,REG1002,Rohit Verma,rohit@example.com,true
3,REG1003,Meera Iyer,meera@example.com,true
```

#### courses.csv
```sh
CSE101,Data Structures,4,Prof. Kumar,SPRING,Computer Science
MAT201,Linear Algebra,3,Dr. Rao,FALL,Mathematics
PHY301,Quantum Physics,4,Dr. Singh,SUMMER,PhysicsS
```

## **Java ME vs Java SE vs Java EE**

| **Edition** | **Purpose**                                           | **Use Cases**                         |
| ----------- | ----------------------------------------------------- | ------------------------------------- |
| **Java ME** | Micro Edition for embedded devices                    | Mobile/IoT applications               |
| **Java SE** | Standard Edition for desktop and console applications | Command-line tools, standalone apps   |
| **Java EE** | Enterprise Edition for server-side applications       | Web applications, APIs, microservices |

---

## **JDK / JRE / JVM Explanation**

- JVM (Java Virtual Machine): Executes Java bytecode

- JRE (Java Runtime Environment): JVM + runtime libraries required to run applications

- JDK (Java Development Kit): JRE + development tools (javac, jar, javadoc)

**Flow:** Java source code → compiled by javac → bytecode → executed by JVM

---

### Acknowledgements
This project was developed with guidance from:

Oracle Java Docs & Tutorials
Java SE 17 Official Docs
VS Code/Eclipse IDE documentation
Mentors & peers for valuable feedback
