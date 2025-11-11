# Reflection Document: Key Experiences and Challenges



## Key Experiences

### 1. Database Design and SQL Operations
I created relational tables for `users` and `calculations` with proper constraints and foreign key relationships. Performing **INSERT**, **SELECT**, **UPDATE**, and **DELETE** operations deepened my understanding of how data flows within a relational model.  
Writing SQL joins to retrieve user-specific calculation data strengthened my grasp of query logic and database relationships.

### 2. Automation and CI/CD Integration
Setting up **GitHub Actions** was one of the most rewarding parts of the project.  
I implemented a workflow that:
- Runs automated tests using `pytest`
- Performs security scans using **Trivy**
- Builds and pushes Docker images to **Docker Hub**
- Supports multi-platform builds using `buildx`

This experience gave me hands-on exposure to **continuous integration and deployment**, which is vital in modern DevOps practices.

---

## Challenges Faced

### 1. Docker Authentication Errors
A major challenge was resolving **Docker login failures** when pushing images to Docker Hub.  
Despite using the correct credentials, the workflow initially failed due to an **invalid access token configuration**.  
I learned to:
- Generate a **Personal Access Token (PAT)** in Docker Hub  
- Configure **GitHub Secrets** properly (`DOCKERHUB_USERNAME`, `DOCKERHUB_TOKEN`)
- Verify successful authentication locally using `docker login`

This debugging process strengthened my ability to troubleshoot authentication and deployment pipelines.

### 2. Database Configuration in CI Environment
Another issue arose while setting up PostgreSQL as a service within GitHub Actions.  
Ensuring the database initialized correctly and matched local configurations required careful management of **environment variables** and **health checks**.  
Through iteration and testing, I achieved a stable setup for automated test execution.

---

## Reflection
This project was a comprehensive learning experience that bridged **data engineering, DevOps, and software development** concepts.  
I learned to approach technical issues systematically—examining logs, validating configurations, and testing iteratively until successful results were achieved.

Beyond technical growth, I improved in:
- **Documentation and reporting**
- **Version control practices**
- **Automation mindset for scalability**

Overall, the project enhanced my understanding of how databases, containers, and CI/CD pipelines work together to build efficient and reliable systems.

---

## Technologies Used
- **PostgreSQL**
- **Docker & Docker Hub**
- **GitHub Actions**
- **Python (pytest)**
- **Trivy Security Scanner**

---


