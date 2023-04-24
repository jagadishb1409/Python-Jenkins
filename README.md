# Installation

There are various methods available to install Jenkins for practicing, but using Docker is highly recommended as it allows you to run multiple containers on your local machine.

## Installation with Docker

To get started with Docker, follow the below steps:

1. Install Docker on your machine.

2. Run the following command to start the Jenkins server:

````console
docker run -p 8080:8080 jenkins/jenkins
````
   Once the installation is complete, you can access Jenkins through localhost:8080.

3. For the first time, Jenkins will ask you to change the password, as shown below:

<img src="https://user-images.githubusercontent.com/63513035/234072140-69e122ae-75ad-41b8-a17f-79a9feb04d65.png" alt="jenkins-password-change-page" width="700"/>

4. Open the command prompt and enter the Docker using the following command:

````console
docker exec -it <container_name> bash
````

5. Upon logging in, use the following command to get the password:

````console
cat /var/jenkins_home/secrets/initialAdminPassword
````

Copy the password and paste it in the Jenkins portal.

6. Install the suggested plugins as shown below:
<img src="https://user-images.githubusercontent.com/63513035/234074062-66640b79-1700-4d9c-9db1-03f2fd81d88e.png" alt="jenkins-suggested-plugins-page" width="700"/>

7. Wait until all the plugins are installed.

8. Fill in all the details for username, password.

9. Keep the Jenkins URL as it is.

10. Now, you should be able to see the Jenkins home page.
