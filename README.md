# azureAKS_deployment
As an alternative, you can run the 05-deploy-apps-via-kubectl.sh script to deploy an instance of the application for each tenant without using Helm. If you use For each tenant, the script will:  Create a namespace Create a deployment for the application instance in the tenant namespace Create a service for the application instance in the tenant namespace Create an ingress in the tenant namespace with {tenant-name}.{domain-name} as hostname Read the public IP address from the ingress Check if an A record exists in the DNS zone on Azure. If yes, the script will delete it. Create an A record with the name of the tenant and the Application Gateway public IP as address
Create a namespace
Create a deployment for the application instance in the tenant namespace
Create a service for the application instance in the tenant namespace
Create an ingress in the tenant namespace with {tenant-name}.{domain-name} as hostname
Read the public IP address from the ingress
Check if an A record exists in the DNS zone on Azure. If yes, the script will delete it.
Create an A record with the name of the tenant and the Application Gateway public IP as address
