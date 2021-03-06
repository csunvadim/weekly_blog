---
layout:     post
title:      Launch ec-2 instance using Terraform
date:       2019-10-25 10:20:18
summary:    Summary for week 9.
categories: jekyll pixyll
---
The following things are needed for this exercuse:
1.) Running Linux machine - such as an ec2 instance.
2.) Access to internet.
3.) AWS root or admin access.

Create an IAM User:
1.) To initialize ec2 from Terraform we need a user that has permission to spin up an ec2.
2.) Go to the IAM and create the appropriate username with ADMIN or full ec2 privileges.
3.) Take a note of the AWS key and AWS secret key of the user to be used later.

Installing Terraform:
1.) On Terraform website, find oppropriate Linux package (x32/x64/ARM) and copy its url.
2.) Use the url from previous step to run "wget {your url}" command, which will download the package.
3.) Unzip the downloaded package, if no longer needed, delete the zipped version file.
4.) Add the following line to ~/.bash_profile "export PATH=$PATH:{path of your installation}", this should link terraform's installation directory.
5.) To apply changed from previous step, run "source ~/.bash_profile", test installation and linking by typing "terraform".


Start an ec2 instance using terraform:
1.) Create your first terraform file (do not forget the .tf extension) "{yourfilename}.tf".
2.) Configure the terraform file with the credentials of created previously, final notebook example:

provider "aws" {
  access_key = "{yourkey}"
  secret_key = "{yoursecret}"
  region     = "{region of choice}
}

resource "aws_instance" "example" {
  ami           = "ami-04b762b4289fba92b"
  instance_type = "t2.micro"
}


3.) Run "terraform init"
4.) Run "terraform apply"
5.) Check ec-2 console, you should see a running instance.
