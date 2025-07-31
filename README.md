# cloudless-app

## quick start 

1. Bootstrap

```bash
curl -sS -L https://$GITHUB_TOKEN@raw.githubusercontent.com/ql4b/cloudless-app/refs/heads/develop/bootstrap \
    | bash -s develop
```

2. Edit the `.env`

```bash
# cloudless-app
AWS_PROFILE=ql4b
AWS_REGION=us-east-1
NAMESPACE=cloudless
NAME=app
```

3. Install serverless

```bash
cd app
npm ci
```

4. Deploy 

```bash
npm run deploy
```

```
✔ Service deployed to stack cloudless-app-staging (31s)

endpoint: GET - https://abcdefghijk.execute-api.us-east-1.amazonaws.com/staging/ip
functions:
  ip: cloudless-app-staging-ip (926 B)

```

```bash
curl -sS https://abcdefghijk.execute-api.us-east-1.amazonaws.com/staging/ip \
    | base64 -d \
    | jq 
```


