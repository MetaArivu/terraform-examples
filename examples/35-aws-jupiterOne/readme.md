# JupiterOne Integration with aws


## Steps done on jupiterOne 


1) create account on https://jupiterone.com/  

2) For Intergating Aws : Go setting option and select Intregation

![MS](https://raw.githubusercontent.com/MetaArivu/terraform-quickstart/main/images/aws-integration.jpg)

3) In intergration page select aws 

4) click on Add the configuration.

![MS](https://raw.githubusercontent.com/MetaArivu/terraform-quickstart/main/images/add-configuration.jpeg)

5) Here you will get the AccountID and external ID

COPY those for future use in terraform script.

![MS](https://raw.githubusercontent.com/MetaArivu/terraform-quickstart/main/images/J1-6-Integration-AWS-Terraform.jpg)


## Terraform Edits


1) Edit main.tf file replace "extId:" with external ID and "acctID:" with AccountID

save the main.tf.

2) terraform init 


3) terraform plan -out output.tf


4) terraform apply output.tf

Here You will create the IAM role for  acessing aws resources by JupiterOne

The output of the result will have arn of the role COPY that for future use.


## Jupiter ADD configuration 


1) Give the Name to the configuration 

2) Paste the role arn we have copied from the output of terraform.

3) save the configuration





