**AWS Cloud Development Kit (CDK)**

- Define your cloud infrastructure using a familiar language;
- The code is "compiled" into a CloudFormation template (JSON/YAML);
- You can therefore deploy infrastructure and application runtime code together;

---

**CDK example**

```python
from aws_cdk import (
    Stack,
    Duration,
    aws_s3 as s3,
    aws_lambda as lambda_,
)
from constructs import Construct


class MyCdkAppStack(Stack):

    def __init__(
        self,
        scope: Construct,
        construct_id: str,
        **kwargs,
    ) -> None:
        super().__init__(scope, construct_id, **kwargs)

        bucket = s3.Bucket(
            self,
            "DataBucket",
            versioned=True,
            block_public_access=s3.BlockPublicAccess.BLOCK_ALL,
        )

        function = lambda_.Function(
            self,
            "MyFunction",
            runtime=lambda_.Runtime.PYTHON_3_12,
            handler="handler.main",
            code=lambda_.Code.from_asset("lambda"),
            timeout=Duration.seconds(30),
        )

        bucket.grant_read_write(function)
```

---
