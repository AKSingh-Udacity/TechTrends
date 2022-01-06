# TechTrends 
Udacity first project of Cloud Native Application Architecture Nanodegree.

In this project,provided am a platform engineer with the main role to package and deploy the application to a Kubernetes platform. 
Throughout this project, I have to use Docker to package the application, and automated the Continuous Integration process with GitHub Actions.
For the release process, I have used Kubernetes declarative manifests, which were templated using Helm. To automated the Continuous Delivery process, finally used ArgoCD

# Brief 
TechTrends is an online website used as a news sharing platform, that enables consumers to access the latest news within the cloud-native ecosystem. In addition to accessing the available articles, readers are able to create new media articles and share them.

Imagine the following scenario: We joined a small team as a Platform Engineer. The team is composed of 2 developers, 1 platform engineer (you), 1 project manager, and 1 manager. The team was assigned with the TechTrends project, aiming to build a fully functional online news sharing platform. The developers in the team are currently working on the first prototype of the TechTrends website. As a platform engineer, we should package and deploy TechTrends to Kubernetes using a CI/CD pipeline.

The web application is written using the Python Flask framework. It uses SQLite, a lightweight disk-based database to store the submitted articles.

Below we can examine the web application component of the techtrends application:
![image](https://user-images.githubusercontent.com/37039539/148359036-6dc94e0b-a691-430a-bfbe-e5aacaff9557.png)
Additionally, the initial sitemap of the website can be found below:
![image](https://user-images.githubusercontent.com/37039539/148359365-2bfac509-f8c9-45ed-8e0f-20bd6a8f6e83.png)

Where:

- About page - presents a quick overview of the TechTrends site

- Index page - contains the content of the main page, with a list of all available posts within TechTrends

- New Post page - provides a form to submit a new post

- 404 page - is rendered when an article ID does not exist is accessed

And lastly, the first prototype of the application is storing and accessing posts from the "POSTS" SQL table. A post entry contains the post ID (primary key), creation timestamp, title, and content. The "POSTS" table schema can be examined below:
![image](https://user-images.githubusercontent.com/37039539/148359858-13810ea5-e7b4-49e6-8fdc-83913d9c8d02.png)

# Project Steps Overview:

1. Apply the best development practices and develop the status and health check endpoints for the TechTrends application.
2. Package the TechTrends application by creating a Dockefile and Docker image.
3. Implement the Continuous Integration practices, by using GitHub Actions to automate the build and push of the Docker image to DockerHub.
4. Construct the Kubernetes declarative manifests to deploy TechTrends to a sandbox namespace within a Kubernetes cluster. The cluster should be provisioned using k3s in a vagrant box.
5. Template the Kubernetes manifests using a Helm chart and provide the input configuration files for staging and production environments.
6. Implement the Continuous Delivery practices, by deploying the TechTrends application to staging and production environments using ArgoCD and the Helm chart.

# Project Requirements:

- Fork the repository [TechTrends application](https://github.com/udacity/nd064_course_1/tree/main/project).
- Install [Python](https://www.python.org/downloads/).
- Install [Docker](https://docs.docker.com/get-docker/).
- Install [Git](https://git-scm.com/downloads).
- Install [Vagrant](https://www.vagrantup.com/downloads).

# Project Checklist Steps
- Access your techtrends on [port](http://127.0.0.1:7111).
- Kubernetes pods, resources creation via k3s.
- Argocd deployment on argocd
- Github Action section of your repository.
- Helm chart execution

