# Serverless Framework - Minimal reproduction of SLS Custom EventBridge rule truncation issue


## Usage

* Deploy to AWS

### Deployment

You need to have an AWS account with the credentials setup correctly.

In order to deploy the example, you need to run the following command:

```
$ serverless deploy
```

### Invocation

After successful deployment, you can invoke the deployed function by using the following command:

```bash
serverless invoke --function hello
```

Which should result in response similar to the following:

```json
{
    "statusCode": 200,
    "body": "{\n  \"message\": \"Go Serverless v2.0! Your function executed successfully!\",\n  \"input\": {}\n}"
}
```

### Local development

You can invoke your function locally by using the following command:

```bash
serverless invoke local --function hello
```

Which should result in response similar to the following:

```
{
    "statusCode": 200,
    "body": "{\n  \"message\": \"Go Serverless v2.0! Your function executed successfully!\",\n  \"input\": \"\"\n}"
}
```
