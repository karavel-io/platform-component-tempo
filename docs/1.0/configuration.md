# Configuration

```hcl
component "tempo" {
  namespace = "tempo"

  # Params default values

  store = "filesystem" # required, storage provider for tempo, available options: "filesystem", "s3"

  # if using s3 for storage, this section is required and must point to an S3 bucket
  s3 = {
    region = ""        # required, bucket region
    bucket = ""        # required, bucket name
    endpoint = ""      # optional, S3 endpoint if different from the default AWS endpoint
    encrypted = true   # optional, enable to use server-side encryption
    insecure = false   # optional, enable to skip server certificate validation
    pathStyle = false  # optional, enable to force path-style requests (eg. minio and similar providers)
    eksRole = ""       # optional, EKS role
    iamRole = ""       # optional, IAM role
  }

  # override if grafana is running in a different namespace
  grafana = {
    namespace: "" # optional
  }
}
```
