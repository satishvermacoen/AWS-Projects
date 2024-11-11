# CI-CD_Pipeline-Jenkins

CI/CD Pipeline with use of Jenkins and other tools:- Maven, Git, Java etc. on the Local Machine(Windows-10)
## Steps--Installation and Configuration.

### Git
- Download-Git-https://git-scm.com/downloads
- Install as Default and Config
![view](./img/ci%20(1).png)
### JAVA
- Download-JAVA- https://www.oracle.com/in/java/technologies/downloads/
- Install as Default.
![view](./img/ci%20(2).png)
#### JAVA Configration on Windows
- Config in Environment User & System Variables an bin path for Java
![view](./img/ci%20(3).png)
```
C:\Program Files\Java\jdk-21
```
![view](./img/ci%20(4).png)
```
C:\Program Files\Java\jdk-21\bin
```
![view](./img/ci%20(5).png)

### MAVEN
- Download-MAVEN- https://maven.apache.org/download.cgi
- Extract on path- C:\DevTools
![view](./img/m%20(1).png)

#### MAVEN Configration on Windows
- Config in Environment System Variables an bin path for MAVEN
![view](./img/m%20(2).png)
```
C:\DevTools\apache-maven-3.9.5
```
![view](./img/m%20(3).png)
```
C:\DevTools\apache-maven-3.9.5\bin
```
![view](./img/m%20(4).png)

## Restart the system ##

### Jenkins
Download-Jenkins- https://Jenkins.apache.org/download.cgi
- Extract on path- C:\DevTools
![view](./img/j.png)

#### Jenkins Configration on Windows
- Config in Environment System Variables an bin path for Jenkins
C:\ProgramData\Jenkins\.jenkins\secrets\initialAdminPassword
```
C:\DevTools\apache-Jenkins-3.9.5
```
![view](./img/m%20(3).png)
```
C:\DevTools\apache-Jenkins-3.9.5\bin
```
![view](./img/m%20(4).png)




## MAVEN JOB, SCHEDULE TASK, POLL SCM.

### JAVA Project clone

```bash
git clone https://github.com/devopsdemoapps/spring-petclinic.git
```
```bash
-  cd # To the directory where you cloned th repo
```
Run command to bulid the java project-

```bash
mvn clean package
```
After that bulid start and it take 10 to 15 min

Now the same bulid through <b>Jenkins</b>

#### Steps

- Open <b>Jenkins</b> through " http://localhost:8080/" 
- login
- Install - <b>MANVEN</b> Plugin
- Config and and Run(screenshoot) step by step
![view](./img/mj%20(1).png)
![view](./img/mj%20(2).png)
![view](./img/mj%20(3).png)
![view](./img/mj%20(4).png)
![view](./img/mj%20(5).png)
![view](./img/mj%20(6).png)
![view](./img/mj%20(7).png)

### This my first bulid job result.

![view](./img/mj%20(8).png)
 
All done for this Projec of GIT, MAVEN, JENKINS.

See you soon...............