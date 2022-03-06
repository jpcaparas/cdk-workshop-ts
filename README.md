# Welcome to your CDK TypeScript project!

You should explore the contents of this project. It demonstrates a CDK app with an instance of a stack (`CdkWorkshopStack`)
which contains an Amazon SQS queue that is subscribed to an Amazon SNS topic.

The `cdk.json` file tells the CDK Toolkit how to execute your app.

## Tutorial  
See [this useful workshop](https://cdkworkshop.com/20-typescript.html) on working with the AWS CDK for Typescript projects.

## Useful commands

 * `npm run build`   compile typescript to js
 * `npm run watch`   watch for changes and compile
 * `npm run test`    perform the jest unit tests
 * `cdk deploy`      deploy this stack to your default AWS account/region
 * `cdk diff`        compare deployed stack with current state
 * `cdk synth`       emits the synthesized CloudFormation template
 
## Local dependencies
This project was developed locally on my machine with the following:

- `cdk` @ `1.129.0 (build fb43f89)`
- `nodejs` @ `v14.19.0`
- (Optional) `cdklocal` @ `1.129.0 (build fb43f89)`
- (Optional) `aws-vault` @ `v6.5.0`

## Gotchas
There are some gotchas that you may encounter along the way:

1. I intentionally was running an older version of `cdk` on this project, because 
I don't want to be switching versions all the time.
2. If you are running `cdklocal` wrapper for [localstack](https://github.com/localstack/localstack), ensure that its 
version is the same as the `cdk` here.
3. It's ideal to use `aws-vault` on this project and if you do use it, ensure that a virtual MFA device 
is assigned to the IAM user, otherwise you'll get exceptions during IAM role creation when deploying the project.

