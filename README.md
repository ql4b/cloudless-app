# cloudless-app

## quick start 

1. Bootstrap

```bash

curl -sS -L https://$GITHUB_TOKEN@raw.githubusercontent.com/ql4b/cloudless-app/refs/heads/develop/bootstrap \
    | bash -s develop

```

2. Edit the `.env`

3. Install serverless

```
cd app
npm ci
```

4. Deploy 

```
npm run deploy 
```


