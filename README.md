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
`     |-------Add JAVA_HOME to system environment path`
     
Install Git SCM </br>

Install Maven </br>
`     |-------Add MAVEN_HOME to system environment path`</br>
     
Goto Jenkins Home -> Manage Jenkins -> Global Tool Configuration  </br>
`     |-------Add JDK, paste the java home path`</br>
`     |-------Add Maven, paste the maven home path`</br>

Create a freestyle project </br>
`     |-------use SCM as git -> provide git repository url`</br>
    
Create a maven based project </br>
`    |-------use SCM as git -> provide git repository url`</br>
`    |-------add Build step -> clean install`</br>
`    |-------click build now`</br>
    
Add Three more plugins</br>
`    |-------1) CheckStyles`</br>
`    |-------2) PMD`</br>
`    |-------3) FindBugs`</br>

Modify the maven based project --> check all check boxes in Build Settings
Add the maven goal as "**clean package checkstyle:checkstyle pmd:pmd findbugs:findbugs**"



# DevOps/Docker

Learn the core fundamentals of Docker by building a Node/Express app with a Mongo & Redis database.

✏️ Course developed by **Sanjeev Thiyagarajan**. Check out his video here: https://www.youtube.com/watch?v=9zUHg7xjIqQ

⭐️ Course Contents ⭐️
***0:00:14 Intro & demo express app***
***0:04:18 Custom Images with Dockerfile***
***0:10:34 Docker image layers & caching***
***0:20:26 Docker networking opening ports***
***0:26:36 Dockerignore file***
***0:31:46 Syncing source code with bind mounts***
***0:45:30 Anonymous Volumes hack***
***0:51:58 Read-Only Bind Mounts***
***0:54:58 Environment variables***
***0:59:16 loading environment variables from file***
***1:01:31 Deleting stale volumes***
***1:04:01 Docker Compose***
***1:21:36 Development vs Production configs***

***Part 02: Working with multiple containers***
***1:44:47 Adding a Mongo Container***
***2:01:48 Communicating between containers***
***2:12:00 Express Config file***
***2:21:45 Container bootup order***
***2:32:26 Building a CRUD application***
***2:51:27 Sign up and Login***
***3:06:57 Authentication with sessions & Redis***
***3:34:36 Architecture Review***
***3:40:48 Nginx for Load balancing to multiple node containers***
***3:54:33 Express CORS***

***Part 03: Moving to Prod***
***3:57:44 Installing docker on Ubuntu(Digital Ocean)***
***4:03:21 Setup Git***
***4:05:37 Environment Variables on Ubuntu***
***4:14:12 Deploying app to production server***
***4:18:57 Pushing changes the hard way***
***4:25:58 Rebuilding Containers***
***4:27:32 Dev to Prod workflow review***
***4:30:50 Improved Dockerhub workflow***
***4:46:10 Automating with watchtower*** 
***4:56:06 Why we need an orchestrator***
***5:03:32 Docker Swarm***
***5:16:13 Pushing changes to Swarm stack***
	
