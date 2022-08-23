> Visit the page docs

- [first AWS CDK app](https://docs.aws.amazon.com/cdk/v2/guide/hello_world.html)

- [AWS CDK Toolkit (cdk command)](https://docs.aws.amazon.com/cdk/v2/guide/cli.html)

- [Bootstrapping](https://docs.aws.amazon.com/cdk/v2/guide/bootstrapping.html)

- `cdk init app --language typescript`

- `cdk bootstrap aws://ACCOUNT-NUMBER/REGION`

  > or

- `cdk bootstrap `

  > if required

- `set CDK_NEW_BOOTSTRAP=2` or `export CDK_NEW_BOOTSTRAP=2`

  > test it

- `npx cdk bootstrap aws://<YOUR_ACCONT_ID>/<YOUR_REGION> --cloudformation-execution-policies arn:aws:iam::aws:policy/AdministratorAccess aws://<YOUR_ACCONT_ID>/<YOUR_REGION>`

  > [Useful commands]()

- `npm run build`
- `cdk ls` //- AwsCdkStack
- `cdk synth`
- `cdk deploy`

- `npm run build` compile typescript to js
- `npm run watch` watch for changes and compile
- `npm run test` perform the jest unit tests
- `cdk deploy` deploy this stack to your default AWS account/region
- `cdk diff` compare deployed stack with current state
- `cdk synth` emits the synthesized CloudFormation template

- `cdk destroy <Stack>`
