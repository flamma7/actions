Practicing GitHub Actions for CI/CD

My goals in order for this project
- GitHub Actions
    - Actions builds and saves docker image to AWS ECS container registry and Docker hub
    - Actions deploys to AWS Fargate
    - [DONE] Use IaC for actions?
    - Add multistage support: dev, staging, master
- AWS
    - configure DNS for api.testdriven.ai to access that AWS Fargate containier
    - set up a program to poll and monitor the traffic to my container
    - add autoscaling of containers
    - **track billing usage and ensure to turn everything off afterwards**
    - integrate with AWS Aurora or Cosmos DB
- Flask
    - add security and use a clean flask routing extension: explore the possible ones and make an opinion
    - add autoscaling
    - add linter and code formatter as an actions step
    - obsfucate the python code
    - semantic-versioning
    - dependency update bot: manages requirements.txt for the docker container??? Woah! 
    - handle migrations with sql alchemy and alembic
- Docker
    - Secure the docker container so people can't read it

Then repeat for GitLab CI/CD

Workflow with Linear
- start an issue by getting the branch name: Ctrl+Shift+.
- first commit put 'part of issue-id' to move it to in-progress
- when done, create a PR and merge it