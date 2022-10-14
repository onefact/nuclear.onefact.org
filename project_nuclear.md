STEP 1: Create New Directory and initialize fly.toml file

mkdir fly-nocodb/
cd fly-nocodb
flyctl launch --image=nocodb/nocodb:latest --no-deploy

STEP 2: Create flyctl volume to store persistent data

flyctl volumes create nocodb_vo

STEP 3: Edit fly.toml file to update the mounts to use created volume

[mounts]
    source="nocodb_vol"
    destination="/usr/app/data"

    
