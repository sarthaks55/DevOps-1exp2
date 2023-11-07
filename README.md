#hello world
Example readme file for my repo

# Define the provider and AWS region
provider "aws" {
  region = "us-east-1"  # Replace with your desired AWS region
}

# Create an EC2 instance
resource "aws_instance" "example_instance" {
  ami           = "ami-0c55b159cbfafe1f0"  # Replace with your desired AMI ID
  instance_type = "t2.micro"               # Replace with your desired instance type
  key_name      = "your-key-pair-name"     # Replace with your SSH key pair name

  tags = {
    Name = "ExampleInstance"
  }
}


{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::exp2s3bucketbuild/*"
        }
    ]
}
