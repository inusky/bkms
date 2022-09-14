```ts
import * as cdk from 'aws-cdk-lib';
import { Construct } from 'constructs';

// "cdk-spa-deploy": "^2.0.0-alpha.1",
import { SPADeploy } from 'cdk-spa-deploy';

export class CdkBackEndStack extends cdk.Stack {
  constructor(scope: Construct, id: string, props?: cdk.StackProps) {
    super(scope, id, props);
    
// create s3 app with cloudFront
    new SPADeploy(this, 'S3CDK-APP').createSiteWithCloudfront({
      indexDoc: 'index.html',
      websiteFolder: '../frontend/build',
    });
  }
}
```
