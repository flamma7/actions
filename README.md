Practicing GitHub Actions for CI/CD

My goals in order for this project
- GitHub Actions
    - Actions builds and saves docker image to AWS ECS container registry and Docker hub
    - Actions deploys to AWS Fargate
- AWS
    - configure DNS for api.testdriven.ai to access that AWS Fargate containier
    - set up a program to poll and monitor the traffic to my container
    - add autoscaling of containers
    - **track billing usage and ensure to turn everything off afterwards**
- Flask
    - add security and clean routing
    - add autoscaling