```
        $ aws -cli --version
        aws-cli/2.7.18 Python/3.9.11 Windows/10 exe/AMD64 prompt/off
```

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

```bash

        $ aws s3 ls
        2022-08-22 17:57:29 sant-demo-image2022
        2022-08-22 18:20:49 sel-demo-sam0220
        2022-08-22 18:21:27 stech-demo-image-test

        $ cdk --version
        2.38.1 (build a5ced21)
```

### [first AWS CDK app](https://docs.aws.amazon.com/cdk/v2/guide/hello_world.html)

- [AWS CDK Toolkit (cdk command)](https://docs.aws.amazon.com/cdk/v2/guide/cli.html)

- `cdk init app --language typescript`

  > cdk bootstrap aws://ACCOUNT-NUMBER/REGION

```ts
// bin/cdk.ts
const envAP = { account: '********', region: 'ap-south-1' };

const app = new cdk.App();
new AwsCdkStack(app, 'AwsCdkStack', {
  env: envAP,
});
```

- `cdk bootstrap `
  set CDK_NEW_BOOTSTRAP=2

- `npm run build`
- `cdk ls` AwsCdkStack
- `cdk synth`
- `cdk deploy`
  ##############################################

```bash
$ aws sts get-caller-identity
        {
        "UserId": "AIDAWHMX6J66NXN7BXADS",
        "Account": "****************",
        "Arn": "arn:aws:iam::****************:user/santosh@serverless"
        }

$ cdk bootstrap aws://****************/ap-south-1

        ⏳  Bootstrapping environment aws://****************/ap-south-1...
        Using default execution policy of 'arn:aws:iam::aws:policy/AdministratorAccess'. Pass '--cloudformation-execution-policies' to customize.
        ✅  Environment aws://****************/ap-south-1 bootstrapped (no changes).

$ aws sts get-caller-identity --profile santosh@serverless
        {
        "UserId": "AIDAWHMX6J66NXN7BXADS",
        "Account": "****************",
        "Arn": "arn:aws:iam::****************:user/santosh@serverless"
        }
```

- `cdk destroy <Stack>`
