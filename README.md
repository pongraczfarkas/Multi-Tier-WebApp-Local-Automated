# Automated Provisioning of a Web Application with Vagrant and VirtualBox

This project demonstrates the automated provisioning of a web application stack using Vagrant and VirtualBox. The application stack includes MySQL, Memcache, RabbitMQ, Tomcat, and Nginx.

#### To check out this project through manual provisioning, [click here](https://github.com/pongraczfarkas/Multi-Tier-WebApp-Local-Manual)

## Diagram

![alt text](https://github.com/pongraczfarkas/Multi-Tier-WebApp-Local-Automated/blob/main/Automated%20provisioning%20diagram.png?raw=true)

## Prerequisites

   - Vagrant (2.3.7)
   - VirtualBox (7.0.8)

## Installation

   1. Install Vagrant and VirtualBox on your development machine.
   2. Clone this repository to your local machine.
   3. Open a terminal window and navigate to the project directory.
   4. Start the Vagrant environment by running the following command:

## Bash

```vagrant up```

This will create and provision the virtual machines for the application stack and automatically install the necessities.
### Application Access

Once the Vagrant environment is up and running, you can access the application as follows:

#### MySQL
```
- Host: 192.168.56.15
- Port: 3306
```
#### Memcache
```
- Host: 192.168.56.14
- Port: 11211
```
#### RabbitMQ
```
- Host: 192.168.56.13
- Port: 5672
```
#### Tomcat
```
- Host: 192.168.56.12
- Port: 8080
```
#### Nginx
```
- Host: 192.168.56.11
- Port: 80
```

## Validating

After going through the Instruction manual, open a browser and type use [this URL](http://192.168.56.11:80)

## Stopping and Removing the Vagrant Environment

To stop the Vagrant environment, run the following command:

```vagrant halt```

To remove the Vagrant environment and all associated virtual machines, run the following command:

```vagrant destroy -f```

## Technologies Used

- Maven 3: A project management and build automation tool for Java projects.
- MySQL 8: A popular open-source relational database management system (RDBMS).
- JDK 11: The latest major version of the Java Development Kit (JDK), the foundational software development kit for Java applications.
- Memcache: An in-memory data store for caching frequently accessed data
- RabbitMQ: A messaging broker for asynchronous communication between applications
- Tomcat: A Java servlet container for running web applications
- Nginx: A high-performance web server for serving static content and load balancing requests
