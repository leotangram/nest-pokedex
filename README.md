<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Execute in develop

1. Clone the repository
2. Ejecute

```
yarn
```

3. Nest CLI installed

```
npm i -g @nestjs/cli
```

4. Raise the database

```
docker-compose up -d
```

5. Clone file **.env.template** and rename to **.env**

6. Fill the variables in **.env** file

7. Run the project in develop

```
yarn start:dev
```

8. Recounstruct the database with seed

```
http://localhost:3000/api/v2/seed
```

## Stack

- NestJS
- TypeORM
- MongoDB
- Docker
- Docker-compose

# Production Build

1. Create file `.env.prod`
2. Fill the variables in `.env.prod` file
3. Create the new image

```
docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build
```
