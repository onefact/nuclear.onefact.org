
1. Create New Directory fly-nocodb and place fly.toml file inside. 
CD to directory in terminal and run

```
mkdir fly-nocodb/
cd fly-nocodb
flyctl launch --image=nocodb/nocodb:latest --no-deploy
```

2. Create flyctl volume named `nocodb_vol` to store persistent data
```
flyctl volumes create nocodb_vol
```

3. Deploy App
```
flyctl deploy
```

4. Open the app:
```
flyctl open
```

5. Create a login for nocodb

## For custom domain

https://fly.io/blog/how-to-custom-domains-with-fly/

Need to add A and AAA records and issue certificate through `flyctl`.

    
