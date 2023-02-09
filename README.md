# MUMU Season2 API Document


## Manual Installation

1.install docker desktop  

2.run command for clone
```bash
git clone https://github.com/mumuSeaosn2/Backend.git
cd Backend
```

3.make .env file (fill the blank)
```
COOKIE_SECRET=
DB_HOST=
DB_USERNAME=
DB_PASSWORD=
DB_DATABASE=
DB_PORT=
GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=
```

4.run command for docker
```bash
docker compose up -d --build
```

5. open docker api container cli and run this command
```
yarn add dotenv
```

6.check out http://localhost:3000/api/docs/

## how to check db status


1.run this command
```
docker exec -it <container-name> bash
mysql -u <user> -p
<user password>
use <database name>

desc <table name>;
or
show tables;
```

## add dummy data
```
docker exec -it mumuseason2-api sh
npx sequelize-cli db:seed:all
```
## License

[MIT](LICENSE)
