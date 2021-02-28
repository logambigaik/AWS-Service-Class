# Read S3 bucket:
![image](https://user-images.githubusercontent.com/54719289/109399751-b7147e80-796a-11eb-802c-0e43e66a3c0d.png)

# Role created:
![image](https://user-images.githubusercontent.com/54719289/109399810-065aaf00-796b-11eb-89a5-0255c1ea53b2.png)

# Create function like trigger whenever file is uploaded into S3:

# Add trigger for S3 (for .csv files uploaded):
![image](https://user-images.githubusercontent.com/54719289/109400285-e8db1480-796d-11eb-8666-f107db20c6fc.png)

# After uploading csv in S3 bucket-cloudwatch log:

![image](https://user-images.githubusercontent.com/54719289/109402411-afa9a100-797b-11eb-8e33-ee1f6d423964.png)

# Check the content in json viewer format (copy the logs from cloudwatch)

![image](https://user-images.githubusercontent.com/54719289/109402582-f2b84400-797c-11eb-92b7-d6d441dbd3a8.png)

  This tree  structure  helps you to do the  code logic like ==> bucket_name=event['Records'][0]['s3']['bucket']['name']

# S3 bucket uploaded:

![image](https://user-images.githubusercontent.com/54719289/109402432-d2d45080-797b-11eb-83cb-48d73fe8ba01.png)

# Lambda function with event print:

![image](https://user-images.githubusercontent.com/54719289/109402447-f4cdd300-797b-11eb-81fd-73601260b0df.png)


# with bucket_name=event['Records'][0]['s3']['bucket']['name']

![image](https://user-images.githubusercontent.com/54719289/109402986-6445c180-7980-11eb-952e-22c810a4f2af.png)

# with filename=event['Records'][0]['s3']['object']['key']


    


