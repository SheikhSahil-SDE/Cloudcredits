# **Cloudcredits**
**DevOps Internship**

**_DevOps project:_**
1. Web Server using Docker.
2. Implement a CI/CD Pipeline. ```https://github.com/SheikhSahil-SDE/Assignment_Projects/actions/workflows/ci.yml```
3. Creating a Chatbot.
4. Jenkins Remoting Project.
5. Building VCS.
6. Deploying a Containerized Web Application.
7. Structuring a Terraform Project.
8. Build a Scalable Application with Kubernetes and Docker.


**_Easy General Structure for a DevOps Project (Short Version)_**

      1. Application Setup
        o Choose a simple app (e.g., Node.js, Python Flask).
        o Host code on Git (GitHub, GitLab).

      2. Continuous Integration (CI)
        o Automate testing using CI tools (e.g., Jenkins, GitHub Actions).
        o Run test cases on code commits.

      3. Containerization
        o Create a Dockerfile to containerize the app.
        o Test locally using Docker.

      4. Continuous Deployment (CD)
        o Deploy to a cloud or server (AWS, Azure, Kubernetes).
        o Automate deployment with CI/CD pipelines.

      5. Monitoring and Logging
        o Monitor using tools like Prometheus and Grafana.
        o Use logging tools like ELK Stack.

      6. Documentation
        o Document steps, tools used, and configurations. 


Example Flow:
```
Commit → CI Pipeline (Build/Test) → Dockerize → Deploy → Monitor.
```


## **ABOUT THE INTERNSHIP**
• Offer Letter 
• Completion Project Certificate 
• Placement Support 
• PPO (Pre Placement Offer)
• Network Opportunity


SOURCR: YouTube | w3schools.com | Udemy

www.cloudcreditstechnologies.in <p> info@cloudcreditstechnologies.in <p>
**9784668018**

# Step 1: Choose 2 Projects

From the list, I recommend starting with these two (combines foundational DevOps skills):
  
Project 1: Web Server using Docker    
Containerize a simple web app (e.g., Node.js/Python Flask).
      
Project 2: Implement a CI/CD Pipeline
Automate testing and deployment for your Dockerized app using GitHub Actions/Jenkins.
  
  Why these?  
  They align with the "General Structure" provided in the PDF.
  They’re beginner-friendly and widely documented.


# Step 2: Set Up GitHub Repository     
Create a repo named Cloudcredits on GitHub.
        Structure it like this:
        
                        Cloudcredits/
                        ├── Project1-Docker-Web-Server/
                        │   ├── app/               # Your application code
                        │   ├── Dockerfile         # Docker configuration
                        │   ├── README.md          # Documentation for the project
                        │   └── ...
                        ├── Project2-CI-CD-Pipeline/
                        │   ├── .github/workflows/ # GitHub Actions pipeline
                        │   ├── Jenkinsfile        # Jenkins pipeline script
                        │   ├── README.md
                        │   └── ...
                        └── ...  

# Step 3: Project 1 – Web Server Using Docker

Tasks:
  1. Build a Simple App:              
      * Use Node.js/Flask to create a "Hello World" app.                  
      * Example Node.js code:
            JavaScript
                    
                    const express = require('express');
                    const app = express();
                    app.get('/', (req, res) => res.send('Hello from Docker!'));
                    app.listen(3000, () => console.log('Server running on port 3000')); 

   2. Containerize with Docker:                  
      * Write a Dockerfile:
            dockerfile
                    
                    FROM node:14
                    WORKDIR /app
                    COPY package*.json ./
                    RUN npm install
                    COPY . .
                    CMD ["node", "app.js"]

       * Build and run locally:
            bash
                           
                  docker build -t my-web-app .
                  docker run -p 3000:3000 my-web-app

        * Push to Docker Hub: Create a Docker Hub account and push your image for later use in CI/CD.

            Documentation: Explain the app, Docker setup, and commands in README.md.

# Step 4: Project 2 – CI/CD Pipeline
 Tasks:

 1. Automate Testing:

    * Add a simple test (e.g., unit test for your app).
      
 2. Set Up GitHub Actions/Jenkins:
      
      * For GitHub Actions:
      
         1. Create .github/workflows/main.yml to automate building, testing, and pushing Docker images.      
         2. Example workflow:
        
                  yaml

                    name: CI/CD Pipeline
                    on: [push]
                    jobs:
                          build:
                            runs-on: ubuntu-latest
                            steps:
                              - uses: actions/checkout@v2
                              - name: Build Docker Image
                                run: docker build -t my-web-app .
                              - name: Run Tests
                                run: docker run my-web-app npm test
 3. Deploy to Cloud:
      * Use AWS/Azure free tier to deploy your Dockerized app (e.g., AWS EC2 or Azure App Service).

Documentation:
      * Describe the pipeline steps, tools, and deployment process in README.md.

Step 5: LinkedIn Demo Videos
      Video 1: Docker Web Server
      Showcase:
      
                  Code structure on GitHub.
                  Docker build process.
                  App running locally/on cloud.

   Hashtags: #Cloudcredits #internship #DevOps.
      

  Video 2: CI/CD Pipeline 
  Showcase:

                  Pipeline triggering on code push.
                  Successful build/test logs.
                  Deployment to the cloud.

  Tag @Cloudcredits in posts.

Step 6: Final Submission
      1. Ensure GitHub repo is public and well-documented.
      2. Submit the repo link via the task form (when shared).
      3. Share LinkedIn video links in the form.

Tools to Learn
                 1. Must-Know: Git, Docker, GitHub Actions/Jenkins, AWS/Azure basics.
                 2. Optional: Kubernetes (for bonus points), Terraform.















