## AWS-CDK

```bash
        PS D:\skyGworkk\dev-explore\AWS-CDK> npm list -g
        C:\Users\skyde\AppData\Roaming\npm
        ├── aws-cdk@2.38.1
        ├── eslint@7.24.0
        ├── minify@9.1.0
        └── npm@8.9.0
```

- `npm install -g aws-cdk` if not foun in `npm list -g` or to check `cdk --version`

- `cdk init app --language typescript`

## Welcome to your CDK TypeScript project

This is a blank project for CDK development with TypeScript.

The `cdk.json` file tells the CDK Toolkit how to execute your app.

## Useful commands

- `npm run build` compile typescript to js
- `npm run watch` watch for changes and compile
- `npm run test` perform the jest unit tests
- `cdk deploy` deploy this stack to your default AWS account/region
- `cdk diff` compare deployed stack with current state
- `cdk synth` emits the synthesized CloudFormation template

## working dynamodb

- `npm install @aws-cdk/aws-dynamodb`

-[aws-cdk-lib.aws_dynamodb module](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_dynamodb-readme.html)

## working lambda

`npm install @aws-cdk/aws-lambda`

## working API Gateway

`npm install @aws-cdk/aws-apigateway`
