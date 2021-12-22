### installation
- copy file called cot-env from fenv folder, paste and renamed to .cot-env to
  root folder
- copy file called cot-envdb from fenv folder, paste and renamed to .cot-envdb
  to root folder
- create folder and file called log folder and inside log folder a
  cotizate_api_application.log file, all inside app folder. 

### build docker
```
 - docker-compose build
```

### up docker
```
 - docker-compose up -d 
```

### migreate db
```
 - docker-compose exec api python3 manage.py migrate --noinput 
```

### create users with commands 
```
 - docker-compose exec api python3 manage.py users
```


### TROUBLESHOOTING
### 1
- if not migrate correnctly, check if folder "migrations" is created in folder
  "core"
- then run makemigrations
- then run migrate
- then create super user
- stop docker, and re-run docker

