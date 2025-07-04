TERRAFORM_VER=`curl -s https://api.github.com/repos/hashicorp/terraform/releases/latest |  grep tag_name | cut -d: -f2 | tr -d \"\,\v | awk '{$1=$1};1'`

wget https://releases.hashicorp.com/terraform/${TERRAFORM_VER}/terraform_${TERRAFORM_VER}_linux_amd64.zip

unzip terraform\_${TERRAFORM_VER}\_linux_amd64.zip

sudo mv terraform /usr/local/bin/

rm terra*.*

vi providers.tf

provider "aws" {

        region = "us-east-1"

        }

Esc :wq

vi newvm.tf

resource "aws_instance" myvm {

        instance_type = "t2.micro"

        ami = "ami-000a08b963606bb82" - replace with your own ami id

tags = {

                Name = "myvm"

                }

}

terraform init

terraform plan

terraform apply
