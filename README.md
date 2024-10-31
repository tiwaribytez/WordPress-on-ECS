#🚀 Deploy a WordPress and MySQL multitier application on AWS ECS using AWS Fargate (i.e Serverless)🚀


🚀Step 1: Navigate to the ECS service.
          Open the AWS Management Console.
          Go to the Amazon ECS service.

Step 2: Create Cluster.
        Click on the Create Cluster Button.

Step 3: Define the cluster name.
        Under the Infrastructure.
        Choose Fargate for the cluster type if it's not already selected.

Step 4: Check that the cluster has been created.

Step 5: Create a New Task Definition
        Go to the Task Definitions section on the left menu.
        Click on Create new Task Definition.

Step 6: Define the Task Name.
        Enter a name for your task defination (e.g., Task_Defination)

Step 7: Select a Launch Type.
        Choose Fargate as the launch type.

Step 8: Define Details for Container 1
        Enter a name for Container 1 (e.g., mysql).
        Enter the Docker image URL (docker.io/mysql).
        Set the port mappings (e.g., port 3306 for MySQL).
        Add Environment Variables for container 1 (mysql)

Step 9: Define Details for Container 2.
        Enter a name for Container 1 (e.g., wordpress).
        Enter the Docker image URL (docker.io/wordpress).
        Set the port mappings (e.g., port 80 for wordpress).
        Set Other Settings as Required.
        Then Click on Create.

Step 10: Check that the task definition is created.

Step 11: Create and Configure a Service.
        Go back to the Clusters section and select your cluster.
        Click on the Services tab, then click Create
        Define the compute option for cluster environment.
        Select the Application Type
        Give a name for service
        Configure additional settings like service discovery, auto-scaling, and
        load balancing.If needed.
        Click Create to deploy the service.

Step 12: Check Service has been created successfully.

Step 13: Check the status of containers by clicking on the
        service and using the path below.

Step 14: Add the Port in Security Group
        Go to the Task (Select your task) > Networking.
        Click on the Security group.
        Edit inbound rules to allow traffic on the necessary ports
        (e.g., HTTP port 80 and MYSQL port 3306).

Step 15: Access WordPress page
        Go back to the ECS service page.
        Find the Tasks tab and locate the running task.
        Copy the public IP address or click on open address.
        Then you will see WordPress page
        Now Enter the require details like database name,username,
        password, host host.

🗝️Setting up an admin account and install WordPress

🎉Sign in into WordPress

⭐Access the WordPress Dashboard
    After sign in, you will be redirected to the WordPress
    dashboard where you can start managing your site.


