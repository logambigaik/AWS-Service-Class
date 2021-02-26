Create EC2 Instance using AWS lambda function:
=============================================


# Step 1 : EC2 Instance creation values:

  First copy the  name of key-value pair : (my case Archu-acc)

![image](https://user-images.githubusercontent.com/54719289/109344249-79ddbd00-7894-11eb-9f7f-c6432dfcef1a.png)

  Copy the AMI ,region and instance_type
  
![image](https://user-images.githubusercontent.com/54719289/109344506-d3de8280-7894-11eb-9861-6ecfbd3077b3.png)


    AMI = 'ami-0ffd774e02309201f'
    INSTANCE_TYPE = 't2.micro'
    KEY_NAME = 'Archu-acc'
    REGION = 'eu-west-2


# Create Lambda function with EC2-Full Access -role :

![image](https://user-images.githubusercontent.com/54719289/109344675-0d16f280-7895-11eb-9dbc-33359c9c4ebf.png)


# Write the function and using Deploy save it. Test the code :

![image](https://user-images.githubusercontent.com/54719289/109344736-27e96700-7895-11eb-8d5d-7350ce54f3fb.png)


# Result:

![image](https://user-images.githubusercontent.com/54719289/109345368-089f0980-7896-11eb-8412-fb297cd32fc3.png)


# Reference:

https://bangmetric.com/creating-an-ec2-instance-with-lambda-in-aws/


# EC2-Instance:

![image](https://user-images.githubusercontent.com/54719289/109345509-44d26a00-7896-11eb-9a62-7ddfffa13696.png)
