# Requirements
1. Install & configure AWS CLI
1. Install & Configure Terraform
1. Install Docker


# Setup
1. Setup everything on AWS side
   1. ```shell script
      cd terraform
      terraform init
      terraform apply -auto-approve;
      cd ..
      ```
1. Populate the DB by uploading the CSV
   1. ```shell script
      aws2 s3 cp ./db/scores.csv s3://vacasa-vhs-jsandlin
      ```
1. 


# TODO
1. Terraform Destroy must be run a couple of times as some dependencies still need linked.
1. No testing
1. Little to no documentation
1. Deploy should be done from Docker / binary repo
1. Frontend doesn't deploy.