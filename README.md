STEP 1: Create New Directory fly-nocodb and place fly.toml file inside. 
CD to directory in terminal and run flyctl launch --image=nocodb/nocodb:latest --no-deploy

mkdir fly-nocodb/
cd fly-nocodb
flyctl launch --image=nocodb/nocodb:latest --no-deploy

STEP 2: Create flyctl volume named nocodb_vol to store persistent data

flyctl volumes create nocodb_vol

STEP 3: Deploy App

flyctl deploy

    
