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
  
  Add Policy:
  
  ![image](https://user-images.githubusercontent.com/54719289/109046405-b5448400-76fa-11eb-85dc-7cbf9c4f4bb8.png)

  



  
  
