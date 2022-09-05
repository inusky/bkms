> Visit the page docs

- [first AWS CDK app](https://docs.aws.amazon.com/cdk/v2/guide/hello_world.html)

- [AWS CDK Toolkit (cdk command)](https://docs.aws.amazon.com/cdk/v2/guide/cli.html)

- [Bootstrapping](https://docs.aws.amazon.com/cdk/v2/guide/bootstrapping.html)

- `cdk init app --language typescript`

- `cdk synth` emits the synthesized CloudFormation template

- `cdk ls` //- AwsCdkStack

- `cdk bootstrap aws://ACCOUNT-NUMBER/REGION`


- `cdk bootstrap --template bootstrap-template.yaml` // if required

```ts
#!/usr/bin/env node
import 'source-map-support/register';
import * as cdk from 'aws-cdk-lib';
import { CdkStack } from '../lib/cdk-stack';

const app = new cdk.App();
new CdkStack(app, 'CdkStack', {
  env: {
    account: process.env.CDK_DEFAULT_ACCOUNT,
    region: process.env.CDK_DEFAULT_REGION,
  },
  /* For more information, see https://docs.aws.amazon.com/cdk/latest/guide/environments.html */
});
```

- `cdk bootstrap `

- `npm run build` compile typescript to js
- `npm run watch` watch for changes and compile
- `npm run test` perform the jest unit tests

- `cdk deploy` deploy this stack to your default AWS account/region

- `cdk diff` compare deployed stack with current state

- `cdk destroy <Stack>`

##############################

> if required

- `set CDK_NEW_BOOTSTRAP=2` or `set CDK_NEW_BOOTSTRAP=2` // once

  > test it

- `cdk bootstrap aws://<YOUR_ACCONT_ID>/<YOUR_REGION> --cloudformation-execution-policies arn:aws:iam::aws:policy/AdministratorAccess aws://<YOUR_ACCONT_ID>/<YOUR_REGION>`

- `cdk bootstrap aws://428204773308/ap-south-1 --cloudformation-execution-policies arn:aws:iam::aws:policy/AdministratorAccess aws://428204773308/ap-south-1`
