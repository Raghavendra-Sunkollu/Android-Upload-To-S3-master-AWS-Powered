# Android-Upload-To-S3-master
 A fully automated architecture built using AWS-Cloud
Provision backend storage
To start provisioning storage resources in the backend, go to your project directory and execute the command:
$ amplify add storage

? Please select from one of the below mentioned services:
    `Content (Images, audio, video, etc.)`
? You need to add auth (Amazon Cognito) to your project in order to add storage for user files. Do you want to add auth now?
    `Yes`
? Do you want to use the default authentication and security configuration?
    `Default configuration`
? How do you want users to be able to sign in?
    `Username`
? Do you want to configure advanced settings?
    `No, I am done.`
? Please provide a friendly name for your resource that will be used to label this category in the project:
    `S3friendlyName`
? Please provide bucket name:
    `storagebucketname`
? Who should have access:
    `Auth and guest users`
? What kind of access do you want for Authenticated users?
    `create/update, read, delete`
? What kind of access do you want for Guest users?
    `create/update, read, delete`
? Do you want to add a Lambda Trigger for your S3 Bucket?
    `No`
    
    
 then type this command
 $ amplify push
  then type this command
 $ amplify init
 
 
 after this command please follow the instruction on the commandline interface


![Screenshot 2021-08-05 22 28 21](https://user-images.githubusercontent.com/71206184/128874802-526f4947-0e47-4971-a282-a16920b01587.png)


![Screenshot 2021-08-05 22 32 00](https://user-images.githubusercontent.com/71206184/128874821-a3d4842c-13d8-4b12-b184-11904b83e58a.png)





please add the python file as a function in AWS lambda this function gets invoked when there is put request in S3,this invokes a trigger which is setup in the infrastructure which writes the results in the DynamoDB database.



![Screenshot 2021-08-05 22 33 59](https://user-images.githubusercontent.com/71206184/128874830-b5f0f6af-8a87-4c1f-8230-d0764f41eef3.png)

![Screenshot 2021-08-05 22 34 43](https://user-images.githubusercontent.com/71206184/128874864-8aae6200-671e-445a-aead-4754ed79ee0a.png)

![Screenshot 2021-08-05 22 37 51](https://user-images.githubusercontent.com/71206184/128874882-f88adaeb-1a39-4b6d-85e6-70d053f156b5.png)
![Screenshot 2021-08-05 22 39 24](https://user-images.githubusercontent.com/71206184/128874892-5fcf77b0-fc4c-4475-a554-7215d36a7815.png)
![Screenshot 2021-08-06 23 18 19](https://user-images.githubusercontent.com/71206184/128874902-7a5fe0c0-4e4f-4a9e-9622-7368ff13d4e2.png)


Configure test event in this manner


![2021-08-10 (1)](https://user-images.githubusercontent.com/71206184/128878029-d7449484-9c3a-46ac-ac87-4b784c9b7e47.png)


 If everythings works fine the architecture works perfectly


 
 
 
 
 
 
