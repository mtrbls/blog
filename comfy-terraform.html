Comfortable Terraform structure for multi-account setup

I have recently been involved in a project where Kubernetes clusters were hosted in AWS environments, and each environment was isolated in its own AWS account.

Although this multi-cluster/multi-environment architecture is standard, the simplest way to manage it all with Terraform isn’t obvious.

Here is what our project look like : 
myCluster/
    main.tf
    provider.tf
    variables.tf
    outputs.tf

What is the simplest way to maintain this across multiple AWS accounts ? 

One folder per environments
The best practice is generally to isolate your environment in their own repo or folder. 
In our case, to keep it simple, we will work in a unique repo.

Let’s say we have three environments: aws-dev, aws-test, aws-prod; each environment will sit in their own folder, with their own terraform state. 

aws-dev/
    myCluster/
aws-test/
    myCluster/
aws-prod/
    myCluster/

Using the folder structure above allows us to run terraform the same way in all environment, simply by changing directory. 

The next question list we face is multiple clusters sitting in the same environment.

One workspace per cluster.

To avoid expanding our environment folder with an ever-increasing amount of cluster, it is recommended to use Terraform workspace.

Terraforrm workspace is terraform state isolation, the same terraform code can be instantiated in different isolated infrastructure. 

Without touching the folder structure above, we can simply create a new workspace named after you cluster : 

cd aws-dev
terraform workspace create cluster-feature-x
terraform init
terraform plan
terraform apply 

NOTE: the assumptiom we make here is that the cluster will be the same as the first one. 
Of course, the local code can be adjusted but the uness it is pushed to your source version control it will conflict with the main terraform code.
Alternatively, git branches can be used to track the terraform code matching  workspace state.
