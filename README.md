# jespson-terraform-backend
# This module will deploy an S3 remote backend for Terraform following the terraform in action book

# USAGE

module "s3backend" {
  source    = "github.com/JespsonSTP/jespson-terraform-backend"      
  namespace = "ProjectName"
}
 
output "s3backend_config" {
  value = module.s3backend.config                      
}