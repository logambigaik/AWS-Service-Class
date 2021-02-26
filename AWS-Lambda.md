# AWS-LAMBDA FOR EC2-STOP Alert:

![image](https://user-images.githubusercontent.com/54719289/109043802-b7f1aa00-76f7-11eb-9ae7-f459cf6882ac.png)

# Step 1: Launch EC2 instance

![image](https://user-images.githubusercontent.com/54719289/109044554-8a593080-76f8-11eb-859b-231bf84760de.png)

# Step 2:  SNS Topic creation

  Create SNS topic and Create Subscription:
  
![image](https://user-images.githubusercontent.com/54719289/109042940-c68b9180-76f6-11eb-8029-dceabe0fa69c.png)
![image](https://user-images.githubusercontent.com/54719289/109042869-afe53a80-76f6-11eb-9ebb-2f72ceb659dc.png)

  Click Pending COnfirmation:
  
![image](https://user-images.githubusercontent.com/54719289/109043206-1702ef00-76f7-11eb-87d8-6b6a304f97d5.png)

![image](https://user-images.githubusercontent.com/54719289/109043423-56c9d680-76f7-11eb-9a5b-84442253a212.png)


  After Subscription:
  
 ![image](https://user-images.githubusercontent.com/54719289/109043596-84168480-76f7-11eb-98c1-8f873f05a6e5.png)

  
# Step 3: IAM Role and Policy creation

  IAM Policy:
  
 ![image](https://user-images.githubusercontent.com/54719289/109044500-7c0b1480-76f8-11eb-8b60-c616c8c03e03.png)

 ![image](https://user-images.githubusercontent.com/54719289/109044848-e6bc5000-76f8-11eb-8475-47a0296fc80a.png)

  Add Additional Permission:
  
  ![image](https://user-images.githubusercontent.com/54719289/109045199-4adf1400-76f9-11eb-93b4-b0fd11a87eb8.png)

  Review the Policy and Click Create Policy:
  
  ![image](https://user-images.githubusercontent.com/54719289/109045422-90034600-76f9-11eb-857e-cd5be9470d14.png)
  ![image](https://user-images.githubusercontent.com/54719289/109045564-c04ae480-76f9-11eb-8e5c-e4dfad639fcd.png)

  IAM Role:
  
  ![image](https://user-images.githubusercontent.com/54719289/109045961-38b1a580-76fa-11eb-943f-118ff0f47068.png)

  Select LAMBDA from AWS Service and CLick Add Permissions:
  
  ![image](https://user-images.githubusercontent.com/54719289/109046079-5bdc5500-76fa-11eb-810f-cc4ea02804dc.png)
  
  Add Policy and CLick Create Role:
  
  ![image](https://user-images.githubusercontent.com/54719289/109046405-b5448400-76fa-11eb-85dc-7cbf9c4f4bb8.png)

  ![image](https://user-images.githubusercontent.com/54719289/109046730-179d8480-76fb-11eb-9e53-5e1ecd77575d.png)
  
  Now Role is created,
  
  ![image](https://user-images.githubusercontent.com/54719289/109046897-4287d880-76fb-11eb-924f-9a3c0ed66f40.png)
  
  Also include AWSLambdaBasicExecutionRole to avoid 403 issue while creating function:
  ![image](https://user-images.githubusercontent.com/54719289/109052887-2471a680-7702-11eb-8a15-f2be6f7664af.png)



# Lambda creation:

![image](https://user-images.githubusercontent.com/54719289/109046897-4287d880-76fb-11eb-924f-9a3c0ed66f40.png)

![image](https://user-images.githubusercontent.com/54719289/109049799-aeb80b80-76fe-11eb-9410-78808d90b233.png)

  Create Function with newly cretaed role
 
 ![image](https://user-images.githubusercontent.com/54719289/109227524-768bf800-77e6-11eb-83e4-abde058671d0.png)

  Double click lambda_function.py,

![image](https://user-images.githubusercontent.com/54719289/109227641-a5a26980-77e6-11eb-9a0d-b4c53ab5257e.png)


  Update the function and test:
  
 ![image](https://user-images.githubusercontent.com/54719289/109230610-24010a80-77eb-11eb-91b0-7864bb38d28c.png)
 
  
    Update Permission inside the function:
    
![image](https://user-images.githubusercontent.com/54719289/109321174-df22b580-7876-11eb-9830-e8a48575e322.png)


![image](https://user-images.githubusercontent.com/54719289/109321512-39bc1180-7877-11eb-9b4c-1d9507cf2cf4.png)

  # Create new IAM role with Lambda:

![image](https://user-images.githubusercontent.com/54719289/109321666-712abe00-7877-11eb-8bff-e96c85c8eb3b.png)
![image](https://user-images.githubusercontent.com/54719289/109322055-d8487280-7877-11eb-83fd-aa8a516c93bc.png)
![image](https://user-images.githubusercontent.com/54719289/109322189-01690300-7878-11eb-8bde-b4e447929085.png)
![image](https://user-images.githubusercontent.com/54719289/109322347-3412fb80-7878-11eb-97b4-a5a73410cc18.png)
![image](https://user-images.githubusercontent.com/54719289/109322685-97049280-7878-11eb-856f-195baae5e0e9.png)




  



  
  
