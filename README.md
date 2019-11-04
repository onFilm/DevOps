# DevOps/Jenkins

### Downloading and running Jenkins
    |-Download Jenkins Web Archieve.
    |-Open up a terminal in the download directory.
    |-Run java -jar jenkins.war --httpPort=8080
    |-Browse to http://localhost:8080.
    |-Follow the instructions to complete the installation. Skip the plugin installation [Recommended]
    
CI, short for **Continuous Integration**, is a software development practice in which all developers merge code changes in a central repository multiple times a day. CD stands for **Continuous Delivery**, which on top of Continuous Integration adds the practice of automating the entire software release process. **Continuous deployment** is a strategy for software releases wherein any code commit that passes the automated testing phase is automatically released into the production environment, making changes that are visible to the software's users

***Continuous Delivery** is the frequent shipping of code to a given environment (such as test or production) via manual release. **Continuous Deployment** is the automated release of code to a production environment.*

#### Post Jenkins setup
Install JDK </br>
Add JAVA_HOME to system environment path </br>
Install Git SCM </br>
Install Maven </br>
Add MAVEN_HOME to system environment path </br>
Goto Jenkins Home -> Manage Jenkins -> Global Tool Configuration  </br>
    Add JDK, paste the java home path </br>
    Add Maven, paste the maven home path </br>

Create a freestyle project </br>
    use SCM as git -> provide git repository url</br>
