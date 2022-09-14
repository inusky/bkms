```ts
#!/usr/bin/env node
import 'source-map-support/register';
import * as cdk from 'aws-cdk-lib';
import { CdkBackEndStack } from '../lib/cdk_back_end-stack';

const app = new cdk.App();
new CdkBackEndStack(app, 'CdkBackEndStack', {
  stackName: 'Rs3DemoApp',
  env: {
    account: process.env.CDK_DEFAULT_ACCOUNT,
    region: process.env.CDK_DEFAULT_REGION,
  },
});
```
