> `aws -cli --version`

```
        $ aws -cli --version
        aws-cli/2.7.18 Python/3.9.11 Windows/10 exe/AMD64 prompt/off
```

> `aws s3 ls`

```bash

        $ aws s3 ls

        2022-08-22 17:57:29 sant-demo-image2022
        2022-08-22 18:20:49 sel-demo-sam0220
        2022-08-22 18:21:27 stech-demo-image-test
```

> `cdk --version` or - `npm list -g`

```bash
        PS D:\skyGworkk\dev-explore\AWS-CDK> npm list -g
        C:\Users\skyde\AppData\Roaming\npm
        ├── aws-cdk@2.38.1
        ├── eslint@7.24.0
        ├── minify@9.1.0
        └── npm@8.9.0
```

> `npm install -g aws-cdk` if require

###########################

> `aws sts get-caller-identity`

```bash
$ aws sts get-caller-identity
        {
        "UserId": "**************",
        "Account": "****************",
        "Arn": "arn:aws:iam::****************:user/santosh@serverless"
        }

$ aws sts get-caller-identity --profile santosh@serverless
        {
        "UserId": "**************",
        "Account": "****************",
        "Arn": "arn:aws:iam::****************:user/santosh@serverless"
        }
```
