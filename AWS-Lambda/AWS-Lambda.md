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

  

# Step 3 : Lambda Function creation:

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

  # Step 4: Create new IAM role with Lambda:

![image](https://user-images.githubusercontent.com/54719289/109321666-712abe00-7877-11eb-8bff-e96c85c8eb3b.png)

![image](https://user-images.githubusercontent.com/54719289/109322055-d8487280-7877-11eb-83fd-aa8a516c93bc.png)

![image](https://user-images.githubusercontent.com/54719289/109322189-01690300-7878-11eb-8bde-b4e447929085.png)

![image](https://user-images.githubusercontent.com/54719289/109322347-3412fb80-7878-11eb-97b4-a5a73410cc18.png)

![image](https://user-images.githubusercontent.com/54719289/109322685-97049280-7878-11eb-856f-195baae5e0e9.png)


# For SNS and EC2 function update the below code (reference link: https://aws.amazon.com/premiumsupport/knowledge-center/start-stop-lambda-cloudwatch/)

    import boto3
    region = 'eu-west-2'
    instances = ['i-0e68334cc3ec4791a']
    ec2 = boto3.client('ec2', region_name=region)

    topic_arn='arn:aws:sns:eu-west-2:136962450893:ec2-stop-alert'
    message = 'ec2 stopped alert'

    sns = boto3.client('sns')

    def lambda_handler(event, context):
        ec2.stop_instances(InstanceIds=instances)
        print('stopped your instances: ' + str(instances))
    
        sns.publish(TopicArn=topic_arn,Message=message)
        print('Topic Arn'+str(topic_arn))
        
        
# Function creation in Lambda:

![image](https://user-images.githubusercontent.com/54719289/109340656-4e0c0880-788f-11eb-97ba-dc26c7313137.png)

# Check the mail for notification












  

  



  
  
