# Terraform Elastic Load Balancer Service Structure

    ├── global                                # contains global resources like S3 and DynamoDB config files
    │   ├── s3                             
    │   │   ├── main.tf                       # contains the terraform configuration to define the S3 and DynamoDB configuration 
    │   │   ├── outputs.tf                    # contains outputs from the terraform configuration
    │   │   ├── variables.tf                  # contains variables used in writing the configuration
    |
    ├── modules                               #  contains modules for the different services 
    │   ├── asg-rolling-update                             
    │   │   ├── main.tf                       # contains the terraform configuration for main ASG
    │   │   ├── outputs.tf                    # contains outputs from the terraform configuration
    │   │   ├── variables.tf                  # contains the variables used in writing this configuration
    │   ├── networking                             
    │   │   ├── main.tf                       # contains the terraform configuration for main network
    │   │   ├── outputs.tf                    # contains outputs from the terraform configuration
    │   │   ├── variables.tf                  # contains the variables used in writing this configuration
    |    
    ├── services                              #  contains modules for the different services 
    │   ├── app                             
    │   │   ├── main.tf                       # contains the terraform configuration for app service
    │   │   ├── outputs.tf                    # contains outputs from the terraform configuration
    │   │   ├── variables.tf                  # contains the variables used in writing this configuration