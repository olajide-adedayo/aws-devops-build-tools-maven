# AWS DevOps Build Tools Project (Maven)

![Project Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![AWS](https://img.shields.io/badge/AWS-Cloud-orange)
![DevOps](https://img.shields.io/badge/DevOps-Project-blue)
![Maven](https://img.shields.io/badge/Maven-Build-red)

## 📌 Project Overview

This project demonstrates the use of Maven as a Build Tool in a DevOps workflow to automate Java application builds, manage dependencies, and generate deployable artifacts.

The project was executed using the vProfile Java web application and focuses on understanding the Maven build lifecycle, artifact generation, and CI/CD readiness.

As part of this hands-on implementation, Maven was used to compile source code, execute tests, package the application, and generate a deployable WAR artifact suitable for deployment in enterprise environments.

## 📌 Business Problem

In modern software development, manually compiling source code, managing dependencies, and packaging applications can be time-consuming and error-prone.

Without a standardized build process, teams often face challenges such as:

- Inconsistent build environments
- Dependency conflicts
- Build failures due to missing libraries
- Difficulty reproducing builds across teams
- Delays in software delivery pipelines

Organizations require reliable and repeatable build automation processes to ensure software can be consistently built, tested, packaged, and prepared for deployment.

Maven addresses these challenges by providing a structured build lifecycle, centralized dependency management, and automated artifact generation for Java applications.

## 🎯 Project Objectives

The main objectives of this project are:

- To understand the Maven build lifecycle in a real-world DevOps workflow
- To automate Java application build processes
- To manage project dependencies using Maven (pom.xml)
- To execute build phases including clean, compile, test, and package
- To generate deployable artifacts (WAR file)
- To prepare the project for CI/CD pipeline integration
- To simulate real-world software build automation practices used in industry

  ## ☁️ AWS Services Used

Although this project is primarily focused on Build Tools, the execution was carried out in a cloud-based development environment.

- AWS CloudShell (Linux-based environment for execution)
- GitHub (Source code version control and repository hosting)

  ---

## 🏗️ Solution Architecture

text
Developer
   ↓
GitHub Repository (Source Code)
   ↓
AWS CloudShell (Linux Environment)
   ↓
Maven Build Tool
   ↓
Build Lifecycle (clean → compile → test → package)
   ↓
WAR Artifact Generation
   ↓
Output Stored in target/ Directory


---

## 🔄 Project Development Workflow

The project was implemented using the following workflow:

### Step 1: Environment Preparation

- Accessed AWS CloudShell environment
- Verified Java installation
- Verified Maven installation

### Step 2: Source Code Setup

- Cloned the vProfile application source code from GitHub
- Navigated to the project directory

### Step 3: Maven Build Execution

Executed the Maven build lifecycle:

bash
mvn clean
mvn compile
mvn test
mvn package
mvn install


### Step 4: Artifact Generation

- Maven successfully compiled the application
- Dependencies were downloaded automatically
- Build artifact was generated successfully

### Step 5: Validation

- Verified build success
- Confirmed WAR artifact generation
- Confirmed artifact availability inside the target directory

---

## 📸 Project Screenshots

### 1. VProfile Project Setup

This screenshot shows the successful cloning and preparation of the vProfile application source code before the build process.

![VProfile Project Setup](screenshots/01-vprofile-build-milestone.png)

---

### 2. Maven Clean Execution

This screenshot shows the successful execution of the Maven clean phase, which removes previous build artifacts and prepares the project for a fresh build.

![Maven Clean Execution](screenshots/02-maven-clean.png)

---

### 3. Maven Build Success

This screenshot shows the successful completion of the Maven build lifecycle, confirming that the application compiled and packaged successfully.

![Maven Build Success](screenshots/03-maven-build-success.png)

---

### 4. WAR Artifact Generation

This screenshot shows the generated WAR artifact inside the target directory, confirming successful packaging and deployment readiness.

![WAR Artifact Generation](screenshots/04-war-artifact.png)

---

---

## 🛠️ Troubleshooting & Root Cause Analysis

During the execution of this project, a few challenges were encountered related to environment setup and build consistency in AWS CloudShell.

### 🔴 Challenge 1: Maven Build Inconsistency

*Issue:*  
Maven build process failed intermittently due to Java runtime mismatch in CloudShell environment.

*Root Cause:*  
Incorrect or inconsistent JAVA_HOME configuration across sessions.

*Solution:*  
Reconfigured JAVA_HOME, validated Java version compatibility, and ensured Maven was aligned with the correct Java runtime before re-executing the build lifecycle.

---

### 🔴 Challenge 2: Artifact Generation Confusion

*Issue:*  
WAR file was not immediately visible after build execution.

*Root Cause:*  
Misunderstanding of Maven build output directory structure.

*Solution:*  
Identified that Maven stores build artifacts in the target/ directory and verified successful WAR generation after build completion.

---

## 📚 Key Learnings

- Maven build lifecycle (clean, compile, test, package, install)
- Java build automation in DevOps workflows
- Dependency management using Maven (pom.xml)
- AWS CloudShell Linux-based development environment
- Debugging build and environment configuration issues
- Understanding artifact generation and storage structure

---

## 📝 Project Documentation

- 📘 Medium Article:  
  https://medium.com/@olajideadedayo230/building-a-java-web-application-with-maven-in-aws-cloudshell-a-complete-devops-build-tools-1a817f316211

- 💻 GitHub Repo:  
  https://github.com/olajide-adedayo/aws-devops-build-tools-maven

- 🔗 LinkedIn:  
  https://www.linkedin.com/in/olajide-adedayo-9126593b3/

---

## 🏁 Conclusion

This project demonstrates practical DevOps implementation using Maven for build automation of a Java web application in AWS CloudShell.

It provides hands-on experience in build lifecycle management, dependency handling, and troubleshooting real-world environment issues, forming a strong foundation for CI/CD pipeline development.

---

## 👤 Author

*Name:* Olajide Adedayo  
*GitHub:* https://github.com/olajide-adedayo  
*LinkedIn:* https://www.linkedin.com/in/olajide-adedayo-9126593b3/  
*Medium:* https://medium.com/@olajideadedayo230
