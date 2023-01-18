Table of Content:
1.	Goal
2.	Pre-Requisites
3.	Process Map
4.	Implementation
5.	Validation

Step-1: Goal
Deploy School web application on Apache server using AWS EC2 instance and automate the process with Jenkins.

Step-2: Pre-Requisites:
1.	Git Client – Git Bash
2.	Version Control Tool - GitHub
3.	CI Tool - Jenkins
4.	Build Tool - Maven
5.	Server – Apache
6.	AWS – EC2, Route53, Certificate Manager

Step-3: Process Map:

![DevOps_Project_04_ProMap](https://user-images.githubusercontent.com/121715127/213105396-1be30827-b83a-445d-ba7a-7d3499e3ad6f.png)

Step-4: Implementation
1. Created remote repository for source code management using version control tool GitHub.
2. Initiated Git repository on AWS EC2 server and integrated with remote repository GitHub by executing Git commands on shell.
3. Installed Jenkins on Linux machine and crated master slave configuration to implement multiple parallel jobs.
4. Integrated GitHub with Jenkins and automated the source code management process by activating GitHub webhooks.
5. Installed Docker on Linux machine (slave) and created docker container & image using docker file.
6. Pushed docker image to Docker Hub remote repository.
7. Docker file created to deploy application on to Apache2 web server. 
8. Configuration of CI/CD Pipeline by integrating Git, GitHub, Jenkins, Docker, AWS and automated the deployment process.
9. All these tools installed on EC2 instances. 
10. Configured AWS EC2 instances, VPC, Security groups, Route table
11. Configured AWS Load balancer and Autoscaling Group to make application always available in the web (to avoid server down issues).
12. DNS and SSL configuration using Route 53 and Certificate Manager

Step-5: Validation
1. Open Domain name in web
2. Make changes in GitHub and Check web for Auto-Update
