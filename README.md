<h2>Steps to deploy and test the application: </h2>

1. Clone the repository
2. Have AWS CLI configured
3. Eksctl should be installed 
4. Create EKS Cluster by running the command: "eksctl create cluster --name orderbird-cluster --region eu-central-1 --nodegroup-name linux-nodes --node-type t2.micro --nodes 2"


Once the cluster is deployed, push the changes to github repo, the pipeline will run automatically.

In Addition, please create below 4 repository variables:
- DOCKER_USER
- DOCKER_PASSWORD
- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY

Let the pipeline do it's thing.