# Guide for Deployment Using AWS CDK
</br>

#### Requirement
1. Node Package Manager, **NPM**
    - https://nodejs.org/en/download
    - https://docs.npmjs.com/downloading-and-installing-node-js-and-npm
2. **AWS CLI**
    - https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
3. AWS Cloud Development Kit, **AWS CDK**

<br>
<br>

## Configure CDK
1. Configure AWS credential
    * Create access key on AWS Account / IAM
        - ![Access key](Configure-CDK/1.Access_Key.png)
    * Open terminal, run `aws configure`
    * Put credential created in AWS Management Console
        - Access Key, Secret Access Key, Specify region, specify output format
        - ![AWS Configure](Configure-CDK/2.AWS_Configure.png)

<br>
<br>

## Destroying Stack
1. Open terminal
2. Go to folder for infrastucture deployment
    * ![Navigate to Infrastructure Folder](Destroy-Stack/1.Stack_Folder.png)
3. List all available stack available in the folder
    * Could be more than 1 stack
    * ![List Stack(s)](Destroy-Stack/2.List_Stack.png)
4. Destroy stack, wait for completion
    * run command `cdk destroy`
        - ![Destroy stack](Destroy-Stack/3.Destroy_CDK.png)
        - ![Destroy stack 2](Destroy-Stack/4.Destroyed_Stack(s).png)
5. Verify stack detroyed on AWS Management Console (CloudFormation)
    * ![Verify destroy](Destroy-Stack/5.Verify.png)
    * ![Verify destroy](Destroy-Stack/6.Verify(2).png)


<br>
<br>

#### References
- https://docs.aws.amazon.com/cdk/v2/guide/home.html
- https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html
- [▶ How To Build a CRUD (TO-DO) App on AWS using FastAPI and Python](https://www.youtube.com/watch?v=iLt00bqp6is)
- [▶ AWS CDK Overview with Stack and Constructs (different examples and use cases)](https://www.youtube.com/watch?v=h_gRGRbOjJ8)
