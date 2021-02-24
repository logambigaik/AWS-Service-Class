# S3 Bucket creation:
  ==================
  
    # Create S3 Bucket and click create bucket

 ![image](https://user-images.githubusercontent.com/54719289/109062698-42dd9f00-770e-11eb-817d-e66a07ed44d6.png) 

 ![image](https://user-images.githubusercontent.com/54719289/109062769-5983f600-770e-11eb-98a7-dded4f65dea8.png)


    # Now select and upload file from local drive to newly created folder called load (after clicking the newly created S3 bucket)
    
 ![image](https://user-images.githubusercontent.com/54719289/109064982-124b3480-7711-11eb-8e0f-9a674fdd5706.png)
 
 
    # Upload Status:
    
  ![image](https://user-images.githubusercontent.com/54719289/109063600-5b01ee00-770f-11eb-814e-f299ed9134b8.png)
  
    # Folder Upload:
    
 ![image](https://user-images.githubusercontent.com/54719289/109065589-d5337200-7711-11eb-8f1d-64c9b9df56a9.png)


 ![image](https://user-images.githubusercontent.com/54719289/109065754-0d3ab500-7712-11eb-9356-fba644499ec6.png)
 
 
  # Create Another bucket:
  
  ![image](https://user-images.githubusercontent.com/54719289/109071928-5d1d7a00-771a-11eb-92bd-06097143e240.png)


# Creating S3 bucket with awscli:
  
  connecting s3 with ec2 required to create either IAM roles&policies or user&Policies
 
  Command to create S3 bucket:
  
    aws s3api create-bucket --bucket my-bucket --region us-east-1
    
    ![image](https://user-images.githubusercontent.com/54719289/109073606-9e168e00-771c-11eb-9574-934d0e2607af.png)
    
    

        Another example:
    
    aws s3api create-bucket --bucket my-bucket --region eu-west-1 --create-bucket-configuration LocationConstraint=eu-west-1

  
  
  




 
 
 

