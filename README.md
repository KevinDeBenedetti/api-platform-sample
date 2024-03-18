# API PLATFORM with external database

## Setup
Clone the repository and create a .env.local with your own values.
### Create .env.local
```dotenv
DATABASE_URL=
HTTP_PORT=
HTTPS_PORT=
HTTP3_PORT=
```

### Start docker
```bash
docker compose --env-file .env.local up -d
```

### Connect with docker database
Add the container to the network of the database
```bash
docker network connect <NETWORK_NAME> api-platform-sample-php-1
```

## Credits
[API Platform repository](https://github.com/api-platform/api-platform)
