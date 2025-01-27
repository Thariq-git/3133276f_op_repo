RP-DV1C04-3133276f

Project Overview:
This project is a DevOps pipeline designed for the RP-DV1C04 coursework assignment. The pipeline automates deploying and testing an index.html file on UAT and PROD environments.

Pipeline Stages:
1. Checkout Code: Retrieves code from the GitHub repository.
2. Build Environment: Sets up the environment for deployment.
3. Deploy to UAT: Deploys index.html to the UAT container.
4. Validate UAT: Verifies the UAT server is operational.
5. Deploy to PROD: Deploys index.html to the PROD container.
6. Validate PROD: Verifies the PROD server is operational.
7. Finalize: Marks the pipeline as complete.

Required Files:
1. 3133276f_jenfile: Contains the Jenkins pipeline definition.
2. 3133276f_index.html: HTML file to replace on the UAT and PROD servers.
3. 3133276f_script: Puppet script for server setup and deployment.

Setup Steps:
1. Clone the repository: git clone https://github.com/youraccount/3133276f_op_repo.git
2. Set up UAT and PROD Docker containers.
3. Configure Jenkins with the Jenkinsfile.
4. Run the pipeline and monitor each stage.

Validation Commands:
- UAT: curl -Is http://svr-uatsvr.localdomain | head -n 1
- PROD: curl -Is http://svr-prodsvr.localdomain | head -n 1

Expected Output: HTTP/1.1 200 OK

Screenshots:
Capture pipeline execution, console output, and index.html before and after deployment.
